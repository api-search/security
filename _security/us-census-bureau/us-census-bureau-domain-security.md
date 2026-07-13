---
api_specs:
- filename: census-data-api-openapi.yml
  format: yaml
  label: Census Data API
  slug: census-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-data-api-openapi.yml
- filename: census-microdata-api-openapi.yml
  format: yaml
  label: Census Microdata API
  slug: census-microdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-microdata-api-openapi.yml
- filename: census-tigerweb-rest-openapi.yml
  format: yaml
  label: TIGERweb REST Services
  slug: census-tigerweb-rest-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-tigerweb-rest-openapi.yml
- filename: census-geocoder-api-openapi.yml
  format: yaml
  label: Census Geocoding Services API
  slug: census-geocoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-geocoder-api-openapi.yml
- filename: census-bds-api-openapi.yml
  format: yaml
  label: Business Dynamics Statistics API
  slug: census-bds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-bds-api-openapi.yml
- filename: census-international-trade-api-openapi.yml
  format: yaml
  label: International Trade API
  slug: census-international-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-international-trade-api-openapi.yml
- filename: census-population-clock-api-openapi.yml
  format: yaml
  label: Population Clock API
  slug: census-population-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-population-clock-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: census.gov
  spf: true
hosts:
- cert_expires: Oct  2 23:56:12 2026 GMT
  host: www.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: tigerweb.geo.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Us Census Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Census Bureau, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Census Bureau
provider_slug: us-census-bureau
slug: us-census-bureau-domain-security
source_filename: us-census-bureau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.census.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.census.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tigerweb.geo.census.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: census.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/security/us-census-bureau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Federal
- Demographics
- Statistics
- Economics
- Geospatial
- Open Data
- Public Sector
---
