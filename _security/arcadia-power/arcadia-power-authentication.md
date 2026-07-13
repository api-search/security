---
api_key_in: []
api_specs:
- filename: arcadia-plug-api-openapi.yml
  format: yaml
  label: Arcadia Plug API
  slug: arcadia-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-plug-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arcadia Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcadia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcadia
provider_slug: arcadia-power
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcadia-plug-api-openapi.yml
  type: http
slug: arcadia-power-authentication
source_filename: arcadia-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcadia-plug-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/arcadia-plug-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/authentication/arcadia-power-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Clean Energy
- Utility Data
- Climate
- Sustainability
- Carbon Accounting
- Solar
- Storage
- EV Charging
- Decarbonization
- Energy Intelligence
---
