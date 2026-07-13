---
api_key_in:
- header
api_specs:
- filename: openapi-charges.yml
  format: yaml
  label: Coinbase Commerce Charges API
  slug: coinbase-commerce-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/openapi/openapi-charges.yml
- filename: openapi-checkouts.yml
  format: yaml
  label: Coinbase Business Checkouts API
  slug: coinbase-business-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/openapi/openapi-checkouts.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/authentication/commerce-coinbase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Crypto Payments
- Cryptocurrency
- Payment Gateway
- Commerce
- Bitcoin
- Ethereum
- USDC
- Webhooks
- Charges
- Checkouts
---
