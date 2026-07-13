---
api_key_in:
- header
api_specs:
- filename: realestateapi-openapi.yml
  format: yaml
  label: RealEstateAPI
  slug: realestateapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Realestateapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealEstateAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RealEstateAPI
provider_slug: realestateapi
scheme_count: 1
schemes:
- description: RealEstateAPI account API key.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/realestateapi-openapi.yml
  type: apiKey
slug: realestateapi-authentication
source_filename: realestateapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/realestateapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: RealEstateAPI account API key.\n  sources:\n  - openapi/realestateapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/authentication/realestateapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- Property Data
- MLS
- Valuation
- Geospatial
- Skip Tracing
- Prop-Tech
---
