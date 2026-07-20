---
api_key_in: []
api_specs:
- filename: fulcrumpro-openapi-original.json
  format: json
  label: Fulcrum Public API
  slug: fulcrum-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/openapi/fulcrumpro-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fulcrumpro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fulcrumpro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fulcrumpro
provider_slug: fulcrumpro
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Your API bearer token generated in System Data > Advanced > Public API Setup
  header: 'Authorization: Bearer <token>'
  name: bearer
  scheme: bearer
  sources:
  - openapi/fulcrumpro-openapi-original.json
  token_management_url: https://developers.fulcrumpro.com/docs/authentication
  type: http
slug: fulcrumpro-authentication
source_filename: fulcrumpro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fulcrumpro-openapi-original.json\ndocs: https://developers.fulcrumpro.com/docs/authentication\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Single scheme. Bearer JWT tokens are generated per Fulcrum site under\n    Business Setup -> System Data -> Advanced -> Public API Setup, with a name,\n    description, and expiration date. Tokens are site-scoped, can be created in\n    multiples, and are revoked by deletion. Sent as `Authorization: Bearer <token>`.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Your API bearer token generated in System Data > Advanced > Public API Setup\n  header: 'Authorization: Bearer <token>'\n  token_management_url: https://developers.fulcrumpro.com/docs/authentication\n  sources:\n  - openapi/fulcrumpro-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/authentication/fulcrumpro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Manufacturing
- ERP
- MES
- Manufacturing Execution
- Job Shop
- CNC Machining
- Sheet Metal
- Inventory
- Purchasing
- Quoting
- Scheduling
---
