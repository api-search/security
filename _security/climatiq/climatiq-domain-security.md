---
api_specs:
- filename: climatiq-autopilot-api-openapi.yml
  format: yaml
  label: Climatiq Autopilot API
  slug: climatiq-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-autopilot-api-openapi.yml
- filename: climatiq-cbam-api-openapi.yml
  format: yaml
  label: Climatiq CBAM API
  slug: climatiq-cbam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-cbam-api-openapi.yml
- filename: climatiq-classifications-api-openapi.yml
  format: yaml
  label: Climatiq Classifications API
  slug: climatiq-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-classifications-api-openapi.yml
- filename: climatiq-computing-api-openapi.yml
  format: yaml
  label: Climatiq Computing API
  slug: climatiq-computing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-computing-api-openapi.yml
- filename: climatiq-energy-api-openapi.yml
  format: yaml
  label: Climatiq Energy API
  slug: climatiq-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-energy-api-openapi.yml
- filename: climatiq-estimate-api-openapi.yml
  format: yaml
  label: Climatiq Estimate API
  slug: climatiq-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-estimate-api-openapi.yml
- filename: climatiq-freight-api-openapi.yml
  format: yaml
  label: Climatiq Freight API
  slug: climatiq-freight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-freight-api-openapi.yml
- filename: climatiq-procurement-api-openapi.yml
  format: yaml
  label: Climatiq Procurement API
  slug: climatiq-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-procurement-api-openapi.yml
- filename: climatiq-reference-api-openapi.yml
  format: yaml
  label: Climatiq Reference API
  slug: climatiq-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-reference-api-openapi.yml
- filename: climatiq-search-api-openapi.yml
  format: yaml
  label: Climatiq Search API
  slug: climatiq-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-search-api-openapi.yml
- filename: climatiq-travel-api-openapi.yml
  format: yaml
  label: Climatiq Travel API
  slug: climatiq-travel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-travel-api-openapi.yml
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
