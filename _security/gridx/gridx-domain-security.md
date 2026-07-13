---
api_specs:
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Engine API
  slug: gridx-rate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Bill Calculation API
  slug: gridx-bill-calculation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Analytics API
  slug: gridx-rate-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX OpenADR Programs API
  slug: gridx-openadr-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gridx.com
  spf: true
hosts:
- cert_expires: Aug 18 13:44:50 2026 GMT
  host: www.gridx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api-calculate-docs.gridx.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: pge-pe-api.gridx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gridx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GridX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GridX
provider_slug: gridx
slug: gridx-domain-security
source_filename: gridx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gridx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:44:50 2026 GMT\n  hsts: false\n- host: api-calculate-docs.gridx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: pge-pe-api.gridx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gridx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/security/gridx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Rate Engine
- Billing
- Rate Analytics
---
