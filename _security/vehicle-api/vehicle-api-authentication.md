---
api_key_in:
- query
api_specs:
- filename: vehicle-api-inventory-api-openapi.yml
  format: yaml
  label: Vehicle API Inventory API
  slug: vehicle-api-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-inventory-api-openapi.yml
- filename: vehicle-api-makes-api-openapi.yml
  format: yaml
  label: Vehicle API Makes API
  slug: vehicle-api-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-makes-api-openapi.yml
- filename: vehicle-api-media-api-openapi.yml
  format: yaml
  label: Vehicle API Media API
  slug: vehicle-api-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-media-api-openapi.yml
- filename: vehicle-api-models-api-openapi.yml
  format: yaml
  label: Vehicle API Models API
  slug: vehicle-api-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-models-api-openapi.yml
- filename: vehicle-api-pricing-api-openapi.yml
  format: yaml
  label: Vehicle API Pricing API
  slug: vehicle-api-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-pricing-api-openapi.yml
- filename: vehicle-api-specs-api-openapi.yml
  format: yaml
  label: Vehicle API Specs API
  slug: vehicle-api-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-specs-api-openapi.yml
- filename: vehicle-api-styles-api-openapi.yml
  format: yaml
  label: Vehicle API Styles API
  slug: vehicle-api-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-styles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vehicle Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vehicle API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vehicle API
provider_slug: vehicle-api
scheme_count: 1
schemes:
- description: Edmunds API key obtained from developer.edmunds.com
  in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/vehicle-api-openapi.yml
  type: apiKey
slug: vehicle-api-authentication
source_filename: vehicle-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vehicle-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Edmunds API key obtained from developer.edmunds.com\n  sources:\n  - openapi/vehicle-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/authentication/vehicle-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Cars
- Edmunds
- Pricing
- Vehicles
---
