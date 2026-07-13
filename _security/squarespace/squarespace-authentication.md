---
api_key_in: []
api_specs:
- filename: squarespace-commerce-api-openapi.yml
  format: yaml
  label: Squarespace Commerce API
  slug: squarespace-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-commerce-api-openapi.yml
- filename: squarespace-orders-api-openapi.yml
  format: yaml
  label: Squarespace Orders API
  slug: squarespace-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-orders-api-openapi.yml
- filename: squarespace-products-api-openapi.yml
  format: yaml
  label: Squarespace Products API
  slug: squarespace-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-products-api-openapi.yml
- filename: squarespace-inventory-api-openapi.yml
  format: yaml
  label: Squarespace Inventory API
  slug: squarespace-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-inventory-api-openapi.yml
- filename: squarespace-profiles-api-openapi.yml
  format: yaml
  label: Squarespace Profiles API
  slug: squarespace-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-profiles-api-openapi.yml
- filename: squarespace-transactions-api-openapi.yml
  format: yaml
  label: Squarespace Transactions API
  slug: squarespace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-transactions-api-openapi.yml
- filename: squarespace-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Squarespace Webhook Subscriptions API
  slug: squarespace-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-webhook-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Squarespace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squarespace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Squarespace
provider_slug: squarespace
scheme_count: 1
schemes:
- description: Authenticate using an API key or OAuth access token. Include the token in the Authorization header as "Bearer YOUR_TOKEN".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/squarespace-commerce-api-openapi.yml
  - openapi/squarespace-inventory-api-openapi.yml
  - openapi/squarespace-orders-api-openapi.yml
  - openapi/squarespace-products-api-openapi.yml
  - openapi/squarespace-profiles-api-openapi.yml
  - openapi/squarespace-transactions-api-openapi.yml
  - openapi/squarespace-webhook-subscriptions-api-openapi.yml
  type: http
slug: squarespace-authentication
source_filename: squarespace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/squarespace-commerce-api-openapi.yml, openapi/squarespace-inventory-api-openapi.yml,\n  openapi/squarespace-orders-api-openapi.yml, openapi/squarespace-products-api-openapi.yml,\n  openapi/squarespace-profiles-api-openapi.yml, openapi/squarespace-transactions-api-openapi.yml,\n  openapi/squarespace-webhook-subscriptions-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate using an API key or OAuth access token. Include the token in the\n    Authorization header as \"Bearer YOUR_TOKEN\".\n  sources:\n  - openapi/squarespace-commerce-api-openapi.yml\n  - openapi/squarespace-inventory-api-openapi.yml\n  - openapi/squarespace-orders-api-openapi.yml\n  - openapi/squarespace-products-api-openapi.yml\n  - openapi/squarespace-profiles-api-openapi.yml\n  - openapi/squarespace-transactions-api-openapi.yml\n  - openapi/squarespace-webhook-subscriptions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/authentication/squarespace-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- E-Commerce
- Marketing
- Payments
- Retail
- Website Builder
- Webhooks
---
