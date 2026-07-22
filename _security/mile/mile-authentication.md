---
api_key_in:
- query
api_specs:
- filename: mile-partner-api-openapi-original.json
  format: json
  label: Mile Partner API
  slug: mile-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-partner-api-openapi-original.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mile secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mile
provider_slug: mile
scheme_count: 2
schemes:
- applied: global
  bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/mile-partner-api-openapi-original.json
  type: http
- description: Access token issued by POST /api/v1/partners/login, passed as the `access_token` query parameter on partner endpoints (products, orders, customers, webhooks, etc.).
  in: query
  name: access_token
  parameter: access_token
  sources:
  - openapi/mile-partner-api-openapi-original.json
  type: apiKey
slug: mile-authentication
source_filename: mile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mile-partner-api-openapi-original.json\ndocs: https://lastmile.milenow.com/partner/api/doc\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  notes: >-\n    Partners authenticate by POSTing credentials to /api/v1/partners/login (user + password\n    query parameters) which returns an access_token. The OpenAPI declares a global HTTP Bearer\n    (JWT) scheme, and in practice the token is also accepted as an `access_token` query\n    parameter on the partner operations.\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: global\n  sources:\n  - openapi/mile-partner-api-openapi-original.json\n- name: access_token\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: >-\n    Access token issued by POST /api/v1/partners/login, passed as the `access_token` query\n    parameter on partner endpoints (products, orders, customers, webhooks, etc.).\n \
  \ sources:\n  - openapi/mile-partner-api-openapi-original.json\nlogin:\n  operation: post_app_apiv1_trackingapi_index\n  path: /api/v1/partners/login\n  method: POST\n  params: [user, password]\n  returns: access_token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/authentication/mile-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Logistics
- Supply Chain
- Last Mile Delivery
- Order Management
- Warehouse Management
- Transportation Management
- Fulfillment
- Shipping
- Webhooks
- Route Optimization
---
