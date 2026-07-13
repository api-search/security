---
api_specs:
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-data-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Assessment API
  slug: attom-data-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM AVM & Valuation API
  slug: attom-data-valuation-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Sales & Deed API
  slug: attom-data-sales-deed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Mortgage API
  slug: attom-data-mortgage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Area & Boundary API
  slug: attom-data-area-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM School API
  slug: attom-data-school-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Community & Neighborhood API
  slug: attom-data-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-data-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Transportation Noise API
  slug: attom-data-transportation-noise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM AllEvents & Snapshot API
  slug: attom-data-allevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Home Equity API
  slug: attom-data-home-equity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: attomdata.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.attomdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.developer.attomdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.gateway.attomdata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attom Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATTOM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ATTOM
provider_slug: attom-data
slug: attom-data-domain-security
source_filename: attom-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.developer.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gateway.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: attomdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/security/attom-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Data
- Real Estate
- Location Data
- Valuation
- AVM
- Assessment
- Mortgage
- Neighborhood
---
