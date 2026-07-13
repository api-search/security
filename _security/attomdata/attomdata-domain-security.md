---
api_specs:
- filename: attom-property-api-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-property-api-openapi.yml
- filename: attom-area-api-openapi.yml
  format: yaml
  label: ATTOM Area API
  slug: attom-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-area-api-openapi.yml
- filename: attom-poi-api-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-poi-api-openapi.yml
- filename: attom-community-api-openapi.yml
  format: yaml
  label: ATTOM Community API
  slug: attom-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-community-api-openapi.yml
- filename: attom-parcel-tiles-api-openapi.yml
  format: yaml
  label: ATTOM Parcel Tiles API
  slug: attom-parcel-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-parcel-tiles-api-openapi.yml
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
name: Attomdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATTOM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ATTOM
provider_slug: attomdata
slug: attomdata-domain-security
source_filename: attomdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.developer.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gateway.attomdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: attomdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/security/attomdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Data
- Property Intelligence
- Mortgage
- Assessment
- AVM
- Foreclosure
- Transactions
- Owner Data
- Building Permits
- Geospatial
- Boundaries
- Demographics
- Neighborhood
- POI
- Insurance
- Mortgage Technology
- PropTech
---
