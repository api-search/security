---
anonymous_access: false
api_key_in: []
api_specs:
- filename: imbawallet-com-auth-api-openapi.yml
  format: yaml
  label: imbawallet-com Auth API
  slug: imbawallet-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-auth-api-openapi.yml
- filename: imbawallet-com-balance-api-openapi.yml
  format: yaml
  label: imbawallet-com Balance API
  slug: imbawallet-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-balance-api-openapi.yml
- filename: imbawallet-com-cards-api-openapi.yml
  format: yaml
  label: imbawallet-com Cards API
  slug: imbawallet-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-cards-api-openapi.yml
- filename: imbawallet-com-catalog-api-openapi.yml
  format: yaml
  label: imbawallet-com Catalog API
  slug: imbawallet-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-catalog-api-openapi.yml
- filename: imbawallet-com-deposit-api-openapi.yml
  format: yaml
  label: imbawallet-com Deposit API
  slug: imbawallet-com-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-deposit-api-openapi.yml
- filename: imbawallet-com-withdrawals-api-openapi.yml
  format: yaml
  label: imbawallet-com Withdrawals API
  slug: imbawallet-com-withdrawals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-withdrawals-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Imbawallet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: imbawallet-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: imbawallet-com
provider_slug: imbawallet-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Access token JWT used in Authorization header.
  scheme: bearer
  type: http
- description: Ed25519 signed assertion JWT exchanged for access token.
  flow: two-step
  tokenUrl: https://imbawallet.com/auth/v1/partner/token
  type: jwt-assertion
slug: imbawallet-com-authentication
source_filename: imbawallet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://api-docs.imbawallet.com/guides/authentication.md\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Access token JWT used in Authorization header.\n  - type: jwt-assertion\n    description: Ed25519 signed assertion JWT exchanged for access token.\n    flow: two-step\n    tokenUrl: https://imbawallet.com/auth/v1/partner/token\n"
source_yaml_url: https://artifacts.apis.io/imbawallet-com/authentication/imbawallet-com-authentication.yml
summary_line: 2 schemes
tags:
- FinTech
- Payments
- Cryptocurrency
- VirtualCards
- Wallet
---
