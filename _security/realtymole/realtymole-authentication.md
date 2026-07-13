---
api_key_in:
- header
api_specs:
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Property Records API
  slug: property-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Rental Estimate API
  slug: rental-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Sale Estimate API
  slug: sale-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Listings API
  slug: listings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Realtymole Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealtyMole secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RealtyMole
provider_slug: realtymole
scheme_count: 1
schemes:
- description: 'RapidAPI subscription key. Requests must also send the header `X-RapidAPI-Host: realty-mole-property-api.p.rapidapi.com`.'
  in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/realtymole-openapi.yml
  type: apiKey
slug: realtymole-authentication
source_filename: realtymole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/realtymole-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: 'RapidAPI subscription key. Requests must also send the header `X-RapidAPI-Host:\n    realty-mole-property-api.p.rapidapi.com`.'\n  sources:\n  - openapi/realtymole-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/authentication/realtymole-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- Property Data
- Rental Estimate
- Valuation
- Listings
---
