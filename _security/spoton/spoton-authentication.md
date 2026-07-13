---
api_key_in:
- header
api_specs:
- filename: spoton-restaurant-pos-export-openapi-original.yml
  format: yaml
  label: SpotOn Restaurant POS Export API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-restaurant-pos-export-openapi-original.yml
- filename: spoton-reserve-openapi-original.yml
  format: yaml
  label: SpotOn Reserve API
  slug: reserve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-reserve-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spoton Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpotOn secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpotOn
provider_slug: spoton
scheme_count: 1
schemes:
- description: API key scoped to specific restaurants.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/spoton-reserve-openapi-original.yml
  - openapi/spoton-restaurant-pos-export-openapi-original.yml
  type: apiKey
slug: spoton-authentication
source_filename: spoton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spoton-reserve-openapi-original.yml, openapi/spoton-restaurant-pos-export-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key scoped to specific restaurants.\n  sources:\n  - openapi/spoton-reserve-openapi-original.yml\n  - openapi/spoton-restaurant-pos-export-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/authentication/spoton-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Point of Sale
- Payments
- Online Ordering
- Reservations
- Reporting
---
