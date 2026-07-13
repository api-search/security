---
api_key_in:
- header
api_specs:
- filename: country-state-city-api-openapi.yml
  format: yaml
  label: Country State City API
  slug: country-state-city-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/openapi/country-state-city-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Country State City Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Country State City API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Country State City API
provider_slug: country-state-city-api
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-CSCAPI-KEY
  sources:
  - openapi/country-state-city-api-openapi.yml
  type: apiKey
slug: country-state-city-api-authentication
source_filename: country-state-city-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/country-state-city-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CSCAPI-KEY\n  sources:\n  - openapi/country-state-city-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/authentication/country-state-city-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Capitals
- Cities
- Countries
- Currencies
- Geography
- Geolocation
- ISO 3166
- JSON
- Phone Codes
- Provinces
- Reference Data
- Regions
- States
- Time Zones
---
