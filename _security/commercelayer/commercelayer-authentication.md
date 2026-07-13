---
api_key_in: []
api_specs:
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer SKUs, Prices & Stock API
  slug: skus-prices-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Orders & Line Items API
  slug: orders-line-items
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Customers & Addresses API
  slug: customers-addresses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Shipments API
  slug: shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Markets API
  slug: markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Promotions API
  slug: promotions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
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
