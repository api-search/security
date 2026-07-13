---
api_key_in:
- header
api_specs:
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Subscriptions API
  slug: ordergroove-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Customers API
  slug: ordergroove-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Orders API
  slug: ordergroove-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Items API
  slug: ordergroove-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Products API
  slug: ordergroove-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Offers and Incentives API
  slug: ordergroove-offers-incentives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Webhooks API
  slug: ordergroove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ordergroove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ordergroove secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ordergroove
provider_slug: ordergroove
scheme_count: 1
schemes:
- description: Application API scope. Send one of the ten store API keys in the x-api-key header for server-to-server requests. Storefront requests use an HMAC-SHA256 signature scoped to a single customer instead (out of band of this scheme).
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/ordergroove-openapi.yml
  type: apiKey
slug: ordergroove-authentication
source_filename: ordergroove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ordergroove-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Application API scope. Send one of the ten store API keys in the x-api-key header\n    for server-to-server requests. Storefront requests use an HMAC-SHA256 signature scoped to\n    a single customer instead (out of band of this scheme).\n  sources:\n  - openapi/ordergroove-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/authentication/ordergroove-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscriptions
- Recurring Commerce
- Relationship Commerce
- eCommerce
- Autoship
- DTC
- Retail
- Subscription Management
---
