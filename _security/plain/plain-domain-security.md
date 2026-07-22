---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plain.com
  spf: true
hosts:
- cert_expires: Sep 26 16:49:33 2026 GMT
  host: www.plain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 00:30:43 2026 GMT
  host: core-api.uk.plain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plain, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plain
provider_slug: plain
slug: plain-domain-security
source_filename: plain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:49:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core-api.uk.plain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:30:43 2026 GMT\n  hsts: null\ndomains:\n- domain: plain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plain/refs/heads/main/security/plain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Support
- Customer Service
- Help Desk
- Support
- SaaS
- GraphQL
- Webhooks
- MCP
- Developer Tools
---
