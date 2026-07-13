---
api_key_in: []
api_specs:
- filename: wayfair-supplier-api.yml
  format: yaml
  label: Wayfair Supplier API
  slug: wayfair-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayfair/refs/heads/main/openapi/wayfair-supplier-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wayfair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wayfair secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wayfair
provider_slug: wayfair
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth2 Bearer token obtained from the /auth/token endpoint. Include as Authorization: Bearer {token} header on all GraphQL requests.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wayfair-supplier-api.yml
  type: http
slug: wayfair-authentication
source_filename: wayfair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wayfair-supplier-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 Bearer token obtained from the /auth/token endpoint. Include as Authorization:\n    Bearer {token} header on all GraphQL requests.'\n  sources:\n  - openapi/wayfair-supplier-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayfair/refs/heads/main/authentication/wayfair-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Furniture
- Home Goods
- Retail
- Suppliers
- GraphQL
---
