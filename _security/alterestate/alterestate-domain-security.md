---
api_specs:
- filename: alterestate-openapi.yml
  format: yaml
  label: AlterEstate API
  slug: alterestate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/openapi/alterestate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alterestate.com
  spf: true
hosts:
- cert_expires: Sep 19 04:05:09 2026 GMT
  host: alterestate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:30:57 2026 GMT
  host: secure.alterestate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alterestate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlterEstate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AlterEstate
provider_slug: alterestate
slug: alterestate-domain-security
source_filename: alterestate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alterestate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:05:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.alterestate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alterestate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/security/alterestate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- CRM
- Property Management
- Lead Management
- Latin America
- SaaS
- Artificial Intelligence
- MCP
---
