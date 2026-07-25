---
api_key_in: []
api_specs:
- filename: commercelayer-addresses-api-openapi.yml
  format: yaml
  label: Commerce Layer Addresses API
  slug: commercelayer-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-addresses-api-openapi.yml
- filename: commercelayer-customers-api-openapi.yml
  format: yaml
  label: Commerce Layer Customers API
  slug: commercelayer-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-customers-api-openapi.yml
- filename: commercelayer-line-items-api-openapi.yml
  format: yaml
  label: Commerce Layer Line Items API
  slug: commercelayer-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-line-items-api-openapi.yml
- filename: commercelayer-markets-api-openapi.yml
  format: yaml
  label: Commerce Layer Markets API
  slug: commercelayer-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-markets-api-openapi.yml
- filename: commercelayer-orders-api-openapi.yml
  format: yaml
  label: Commerce Layer Orders API
  slug: commercelayer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-orders-api-openapi.yml
- filename: commercelayer-payment-methods-api-openapi.yml
  format: yaml
  label: Commerce Layer Payment Methods API
  slug: commercelayer-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-payment-methods-api-openapi.yml
- filename: commercelayer-prices-api-openapi.yml
  format: yaml
  label: Commerce Layer Prices API
  slug: commercelayer-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-prices-api-openapi.yml
- filename: commercelayer-promotions-api-openapi.yml
  format: yaml
  label: Commerce Layer Promotions API
  slug: commercelayer-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-promotions-api-openapi.yml
- filename: commercelayer-shipments-api-openapi.yml
  format: yaml
  label: Commerce Layer Shipments API
  slug: commercelayer-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-shipments-api-openapi.yml
- filename: commercelayer-skus-api-openapi.yml
  format: yaml
  label: Commerce Layer SKUs API
  slug: commercelayer-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-skus-api-openapi.yml
- filename: commercelayer-stock-items-api-openapi.yml
  format: yaml
  label: Commerce Layer Stock Items API
  slug: commercelayer-stock-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-stock-items-api-openapi.yml
- filename: commercelayer-webhooks-api-openapi.yml
  format: yaml
  label: Commerce Layer Webhooks API
  slug: commercelayer-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Commercelayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commerce Layer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commerce Layer
provider_slug: commercelayer
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth2 access token obtained from https://auth.commercelayer.io/oauth/token (client_credentials, password, authorization_code, refresh_token, or JWT bearer grant). Passed as Authorization: Bearer {access_token}. Tokens may carry a market or stock_location scope.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commercelayer-openapi.yml
  type: http
slug: commercelayer-authentication
source_filename: commercelayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commercelayer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token obtained from https://auth.commercelayer.io/oauth/token\n    (client_credentials, password, authorization_code, refresh_token, or JWT bearer grant).\n    Passed as Authorization: Bearer {access_token}. Tokens may carry a market or stock_location\n    scope.'\n  sources:\n  - openapi/commercelayer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/authentication/commercelayer-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Headless
- Composable
- eCommerce
- JSON:API
- Orders
---
