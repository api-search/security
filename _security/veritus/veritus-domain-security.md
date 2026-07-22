---
api_specs:
- filename: veritus-openapi.json
  format: json
  label: Veritus API
  slug: veritus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritus/refs/heads/main/openapi/veritus-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veritus.com
  spf: true
hosts:
- cert_expires: Sep 28 14:53:00 2026 GMT
  host: veritus.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:17:58 2026 GMT
  host: sandbox.veritus.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veritus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veritus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Veritus
provider_slug: veritus
slug: veritus-domain-security
source_filename: veritus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veritus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:53:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: sandbox.veritus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:17:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: veritus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritus/refs/heads/main/security/veritus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Consumer Lending
- Collections
- AI Agents
- Voice AI
- Communications
- Compliance
---
