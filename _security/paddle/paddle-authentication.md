---
api_key_in: []
api_specs:
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Products API
  slug: paddle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Prices API
  slug: paddle-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Customers API
  slug: paddle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Subscriptions API
  slug: paddle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Transactions API
  slug: paddle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Adjustments API
  slug: paddle-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Discounts API
  slug: paddle-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Notifications API
  slug: paddle-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paddle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paddle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paddle
provider_slug: paddle
scheme_count: 1
schemes:
- description: 'Authenticate with your Paddle API key passed in the Authorization header with the Bearer prefix, e.g. `Authorization: Bearer pdl_live_apikey_...`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paddle-openapi.yml
  type: http
slug: paddle-authentication
source_filename: paddle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paddle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with your Paddle API key passed in the Authorization header with\n    the Bearer prefix, e.g. `Authorization: Bearer pdl_live_apikey_...`.'\n  sources:\n  - openapi/paddle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/authentication/paddle-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Payments
- Subscriptions
- Merchant of Record
- SaaS
---
