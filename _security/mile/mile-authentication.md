---
api_key_in:
- query
api_specs:
- filename: mile-aramex-api-openapi.yml
  format: yaml
  label: Mile Aramex API
  slug: mile-aramex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-aramex-api-openapi.yml
- filename: mile-customers-api-openapi.yml
  format: yaml
  label: Mile Customers API
  slug: mile-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-customers-api-openapi.yml
- filename: mile-debug-api-openapi.yml
  format: yaml
  label: Mile Debug API
  slug: mile-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-debug-api-openapi.yml
- filename: mile-drivers-api-openapi.yml
  format: yaml
  label: Mile Drivers API
  slug: mile-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-drivers-api-openapi.yml
- filename: mile-export-api-openapi.yml
  format: yaml
  label: Mile Export API
  slug: mile-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-export-api-openapi.yml
- filename: mile-login-api-openapi.yml
  format: yaml
  label: Mile Login API
  slug: mile-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-login-api-openapi.yml
- filename: mile-order-api-openapi.yml
  format: yaml
  label: Mile Order API
  slug: mile-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-api-openapi.yml
- filename: mile-order-optimization-api-openapi.yml
  format: yaml
  label: Mile Order Optimization API
  slug: mile-order-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-optimization-api-openapi.yml
- filename: mile-order-webhook-api-openapi.yml
  format: yaml
  label: Mile Order Webhook API
  slug: mile-order-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-webhook-api-openapi.yml
- filename: mile-order-with-dynamic-merchant-api-openapi.yml
  format: yaml
  label: Mile Order With Dynamic Merchant API
  slug: mile-order-with-dynamic-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-with-dynamic-merchant-api-openapi.yml
- filename: mile-payment-terms-api-openapi.yml
  format: yaml
  label: Mile Payment Terms API
  slug: mile-payment-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-payment-terms-api-openapi.yml
- filename: mile-products-api-openapi.yml
  format: yaml
  label: Mile Products API
  slug: mile-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-products-api-openapi.yml
- filename: mile-promotion-bundle-api-openapi.yml
  format: yaml
  label: Mile Promotion Bundle API
  slug: mile-promotion-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-promotion-bundle-api-openapi.yml
- filename: mile-routes-api-openapi.yml
  format: yaml
  label: Mile Routes API
  slug: mile-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-routes-api-openapi.yml
- filename: mile-settlement-webhook-api-openapi.yml
  format: yaml
  label: Mile Settlement Webhook API
  slug: mile-settlement-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-settlement-webhook-api-openapi.yml
- filename: mile-vehicles-api-openapi.yml
  format: yaml
  label: Mile Vehicles API
  slug: mile-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-vehicles-api-openapi.yml
- filename: mile-warehouse-inbound-orders-api-openapi.yml
  format: yaml
  label: Mile Warehouse Inbound Orders API
  slug: mile-warehouse-inbound-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-warehouse-inbound-orders-api-openapi.yml
- filename: mile-webhooks-api-openapi.yml
  format: yaml
  label: Mile Webhooks API
  slug: mile-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-webhooks-api-openapi.yml
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
- Webhook
- Route Optimization
---
