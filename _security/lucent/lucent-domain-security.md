---
api_specs:
- filename: lucent-openapi-original.json
  format: json
  label: Lucent API
  slug: lucent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/openapi/lucent-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucenthq.com
  spf: true
hosts:
- cert_expires: Oct  9 10:18:57 2026 GMT
  host: lucenthq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 12:34:07 2026 GMT
  host: docs.lucenthq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 09:42:25 2026 GMT
  host: app.lucenthq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucent, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucent
provider_slug: lucent
slug: lucent-domain-security
source_filename: lucent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:18:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lucenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:34:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.lucenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lucenthq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/security/lucent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Session Replay
- Product Analytics
- Bug Detection
- Observability
- Artificial Intelligence
- Developer Tools
- MCP
- Webhooks
---
