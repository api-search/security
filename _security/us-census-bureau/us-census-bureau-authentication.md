---
api_key_in:
- query
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
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Census Bureau Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Census Bureau secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: US Census Bureau
provider_slug: us-census-bureau
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/census-bds-api-openapi.yml
  - openapi/census-data-api-openapi.yml
  - openapi/census-international-trade-api-openapi.yml
  - openapi/census-microdata-api-openapi.yml
  type: apiKey
slug: us-census-bureau-authentication
source_filename: us-census-bureau-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/census-bds-api-openapi.yml, openapi/census-data-api-openapi.yml, openapi/census-international-trade-api-openapi.yml,\n  openapi/census-microdata-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/census-bds-api-openapi.yml\n  - openapi/census-data-api-openapi.yml\n  - openapi/census-international-trade-api-openapi.yml\n  - openapi/census-microdata-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/authentication/us-census-bureau-authentication.yml
summary_line: apiKey · 1 scheme
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
