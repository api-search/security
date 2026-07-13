---
api_specs:
- filename: emitwise-api-openapi.yml
  format: yaml
  label: Emitwise API
  slug: emitwise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emitwise.com
  spf: true
hosts:
- cert_expires: Oct  2 01:25:52 2026 GMT
  host: emitwise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: docs.emitwise.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.emitwise.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Emitwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emitwise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Emitwise
provider_slug: emitwise
slug: emitwise-domain-security
source_filename: emitwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emitwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.emitwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.emitwise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: emitwise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/security/emitwise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Accounting
- Greenhouse Gas
- Scope 3
- Supply Chain Emissions
- Product Carbon Footprint
- Sustainability
- ESG
- CDP
- CSRD
- GHG Protocol
- Climate
- Procurement
- AI
---
