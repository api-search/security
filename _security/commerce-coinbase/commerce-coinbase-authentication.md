---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: commerce-coinbase-charges-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Charges API
  slug: commerce-coinbase-charges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-charges-api-openapi.yml
- filename: commerce-coinbase-checkouts-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Checkouts API
  slug: commerce-coinbase-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-checkouts-api-openapi.yml
- filename: commerce-coinbase-events-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Events API
  slug: commerce-coinbase-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-events-api-openapi.yml
- filename: commerce-coinbase-webhooks-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Webhooks API
  slug: commerce-coinbase-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-webhooks-api-openapi.yml
- filename: commerce-coinbase-account-management-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Account Management API
  slug: commerce-coinbase-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-account-management-api-openapi.yml
- filename: commerce-coinbase-authentication-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Authentication API
  slug: commerce-coinbase-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-authentication-api-openapi.yml
- filename: commerce-coinbase-combo-books-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Combo Books API
  slug: commerce-coinbase-combo-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-combo-books-api-openapi.yml
- filename: commerce-coinbase-market-data-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Market Data API
  slug: commerce-coinbase-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-market-data-api-openapi.yml
- filename: commerce-coinbase-session-management-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Session Management API
  slug: commerce-coinbase-session-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-session-management-api-openapi.yml
- filename: commerce-coinbase-subscription-management-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Subscription Management API
  slug: commerce-coinbase-subscription-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-subscription-management-api-openapi.yml
- filename: commerce-coinbase-supporting-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Supporting API
  slug: commerce-coinbase-supporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-supporting-api-openapi.yml
- filename: commerce-coinbase-trading-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Trading API
  slug: commerce-coinbase-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-trading-api-openapi.yml
- filename: commerce-coinbase-wallet-api-openapi.yml
  format: yaml
  label: Coinbase Commerce Wallet API
  slug: commerce-coinbase-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerce-coinbase/openapi/commerce-coinbase-wallet-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Commerce Coinbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coinbase Commerce secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coinbase Commerce
provider_slug: commerce-coinbase
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-CC-Api-Key
  sources:
  - openapi/openapi-charges.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT signed with your CDP API Key Secret. See https://docs.cdp.coinbase.com/coinbase-business/authentication-authorization/api-key-authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi-checkouts.yml
  type: http
slug: commerce-coinbase-authentication
source_filename: commerce-coinbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-charges.yml, openapi/openapi-checkouts.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CC-Api-Key\n  sources:\n  - openapi/openapi-charges.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT signed with your CDP API Key Secret. See https://docs.cdp.coinbase.com/coinbase-business/authentication-authorization/api-key-authentication\n  sources:\n  - openapi/openapi-checkouts.yml\n"
source_yaml_url: https://artifacts.apis.io/commerce-coinbase/authentication/commerce-coinbase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Crypto Payments
- Cryptocurrency
- Payment Gateway
- Commerce
- Bitcoin
- Ethereum
- USDC
- Webhook
- Charges
- Checkout
---
