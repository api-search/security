---
api_key_in: []
api_specs:
- filename: 99minutos-api-v3-openapi.json
  format: json
  label: 99minutos API v3
  slug: 99minutos-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99minutos-api-v3-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 99 Minutos Authentication
name_suffix: Authentication
oauth_flows: []
overview: 99 Minutos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 99 Minutos
provider_slug: 99-minutos
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: AuthJWT
  scheme: bearer
  sources:
  - openapi/99minutos-api-v3-openapi.json
  type: http
slug: 99-minutos-authentication
source_filename: 99-minutos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/99minutos-api-v3-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AuthJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/99minutos-api-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/authentication/99-minutos-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Last Mile Delivery
- Shipping
- Ecommerce
- Fulfillment
- Freight
- Tracking
- Webhooks
- Latin America
- Mexico
---
