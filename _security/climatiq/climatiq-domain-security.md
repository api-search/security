---
api_specs:
- filename: climatiq-openapi.yml
  format: yaml
  label: Climatiq API
  slug: climatiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: climatiq.io
  spf: true
hosts:
- cert_expires: Aug 26 16:43:36 2026 GMT
  host: www.climatiq.io
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.climatiq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climatiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climatiq, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Climatiq
provider_slug: climatiq
slug: climatiq-domain-security
source_filename: climatiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.climatiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 16:43:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.climatiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: climatiq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/security/climatiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Energy
- Environment
- GHG Protocol
- Sustainability
---
