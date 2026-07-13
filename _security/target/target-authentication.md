---
api_key_in: []
api_specs:
- filename: target-target-api-openapi.yml
  format: yaml
  label: Target API
  slug: target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-target-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Target Authentication
name_suffix: Authentication
oauth_flows: []
overview: target secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: target
provider_slug: target
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/target-target-api-openapi.yml
  type: http
slug: target-authentication
source_filename: target-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/target-target-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/target-target-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/authentication/target-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 100
- E-Commerce
- Retail
- Products
- Inventory
- Fortune 100
- Stores
- Orders
---
