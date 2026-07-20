---
api_key_in: []
api_specs:
- filename: cargomatic-openapi-original.yml
  format: yaml
  label: Cargomatic Public API
  slug: cargomatic-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargomatic/refs/heads/main/openapi/cargomatic-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cargomatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cargomatic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cargomatic
provider_slug: cargomatic
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cargomatic-openapi-original.yml
  type: http
slug: cargomatic-authentication
source_filename: cargomatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cargomatic-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cargomatic-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargomatic/refs/heads/main/authentication/cargomatic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Freight
- Drayage
- Transportation
- Supply Chain
- Shipping
- Trucking
- Marketplace
- Intermodal
---
