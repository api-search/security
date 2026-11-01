---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chimoney-account-api-openapi.yml
  format: yaml
  label: Chimoney Account API
  slug: chimoney-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-account-api-openapi.yml
- filename: chimoney-info-api-openapi.yml
  format: yaml
  label: Chimoney Info API
  slug: chimoney-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-info-api-openapi.yml
- filename: chimoney-interledger-api-openapi.yml
  format: yaml
  label: Chimoney Interledger API
  slug: chimoney-interledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-interledger-api-openapi.yml
- filename: chimoney-multicurrency-wallets-api-openapi.yml
  format: yaml
  label: Chimoney MultiCurrency Wallets API
  slug: chimoney-multicurrency-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-multicurrency-wallets-api-openapi.yml
- filename: chimoney-payments-api-openapi.yml
  format: yaml
  label: Chimoney Payments API
  slug: chimoney-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-payments-api-openapi.yml
- filename: chimoney-payouts-api-openapi.yml
  format: yaml
  label: Chimoney Payouts API
  slug: chimoney-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-payouts-api-openapi.yml
- filename: chimoney-redeem-api-openapi.yml
  format: yaml
  label: Chimoney Redeem API
  slug: chimoney-redeem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-redeem-api-openapi.yml
- filename: chimoney-wallet-api-openapi.yml
  format: yaml
  label: Chimoney Wallet API
  slug: chimoney-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-wallet-api-openapi.yml
- filename: chimoney-agents-api-openapi.yml
  format: yaml
  label: Chimoney Agents API
  slug: chimoney-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-agents-api-openapi.yml
- filename: chimoney-ai-api-openapi.yml
  format: yaml
  label: Chimoney AI API
  slug: chimoney-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-ai-api-openapi.yml
- filename: chimoney-beneficiary-api-openapi.yml
  format: yaml
  label: Chimoney Beneficiary API
  slug: chimoney-beneficiary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-beneficiary-api-openapi.yml
- filename: chimoney-pass-through-api-openapi.yml
  format: yaml
  label: Chimoney Pass Through API
  slug: chimoney-pass-through-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-pass-through-api-openapi.yml
- filename: chimoney-passport-api-openapi.yml
  format: yaml
  label: Chimoney Passport API
  slug: chimoney-passport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-passport-api-openapi.yml
- filename: chimoney-sub-account-api-openapi.yml
  format: yaml
  label: Chimoney Sub Account API
  slug: chimoney-sub-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimoney/openapi/chimoney-sub-account-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chimoney Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chimoney secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chimoney
provider_slug: chimoney
scheme_count: 1
schemes:
- description: API key issued self-serve from the Chimoney developer dashboard (https://dash.chimoney.io/developers). Passed on every request in the `X-API-KEY` HTTP header. A separate sandbox key and host (https://api-v2-sandbox.chimoney.io) are available for testing; production is https://api.chimoney.io.
  in: header
  name: apiKeyAuth
  parameterName: X-API-KEY
  sources:
  - openapi/chimoney-openapi.yml
  - https://chimoney.readme.io/reference/authentication
  type: apiKey
slug: chimoney-authentication
source_filename: chimoney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/chimoney-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: X-API-KEY\n  description: 'API key issued self-serve from the Chimoney developer dashboard\n    (https://dash.chimoney.io/developers). Passed on every request in the `X-API-KEY`\n    HTTP header. A separate sandbox key and host (https://api-v2-sandbox.chimoney.io)\n    are available for testing; production is https://api.chimoney.io.'\n  sources:\n  - openapi/chimoney-openapi.yml\n  - https://chimoney.readme.io/reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/chimoney/authentication/chimoney-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payouts
- Disbursements
- Payments
- Africa
- Global Payouts
- Wallets
- Multi-Currency
- Gift Cards
- Mobile Money
- Fintech
---
