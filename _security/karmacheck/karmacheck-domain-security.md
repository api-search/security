---
api_specs:
- filename: karmacheck-api-openapi.yml
  format: yaml
  label: KarmaCheck API
  slug: karmacheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/openapi/karmacheck-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: karmacheck.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: karmacheck.io
  spf: true
hosts:
- cert_expires: Sep 29 21:16:07 2026 GMT
  host: www.karmacheck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:09:39 2026 GMT
  host: developer.karmacheck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api.karmacheck.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karmacheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KarmaCheck, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KarmaCheck
provider_slug: karmacheck
slug: karmacheck-domain-security
source_filename: karmacheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.karmacheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.karmacheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.karmacheck.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: karmacheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: karmacheck.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karmacheck/refs/heads/main/security/karmacheck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Credential Verification
- Motor Vehicle Records
- Occupational Health Screening
- Drug Screening
- HR Tech
- Staffing
- Healthcare
- Compliance
- FCRA
- Adjudication
- Webhook
- MCP Server
- agent-native
---
