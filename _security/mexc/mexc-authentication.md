---
api_key_in:
- header
api_specs:
- filename: mexc-accounts-and-transactions-api-openapi.yml
  format: yaml
  label: MEXC Accounts and Transactions API
  slug: mexc-accounts-and-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-accounts-and-transactions-api-openapi.yml
- filename: mexc-eft-api-openapi.yml
  format: yaml
  label: MEXC EFT API
  slug: mexc-eft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-eft-api-openapi.yml
- filename: mexc-margin-api-openapi.yml
  format: yaml
  label: MEXC Margin API
  slug: mexc-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-margin-api-openapi.yml
- filename: mexc-market-date-endpoints-api-openapi.yml
  format: yaml
  label: MEXC Market Date Endpoints API
  slug: mexc-market-date-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-market-date-endpoints-api-openapi.yml
- filename: mexc-parent-child-account-api-openapi.yml
  format: yaml
  label: MEXC Parent child account API
  slug: mexc-parent-child-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-parent-child-account-api-openapi.yml
- filename: mexc-quote-api-openapi.yml
  format: yaml
  label: MEXC Quote API
  slug: mexc-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-quote-api-openapi.yml
- filename: mexc-rebate-api-openapi.yml
  format: yaml
  label: MEXC Rebate API
  slug: mexc-rebate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-rebate-api-openapi.yml
- filename: mexc-spot-account-trade-api-openapi.yml
  format: yaml
  label: MEXC Spot Account/Trade API
  slug: mexc-spot-account-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-spot-account-trade-api-openapi.yml
- filename: mexc-wallet-api-openapi.yml
  format: yaml
  label: MEXC Wallet API
  slug: mexc-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-wallet-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mexc Authentication
name_suffix: Authentication
oauth_flows: []
overview: MEXC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MEXC
provider_slug: mexc
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-MEXC-APIKEY
  sources:
  - openapi/mexc-futures-rest-api-openapi.json
  - openapi/mexc-spot-rest-api-openapi.json
  type: apiKey
slug: mexc-authentication
source_filename: mexc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mexc-futures-rest-api-openapi.json, openapi/mexc-spot-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-MEXC-APIKEY\n  sources:\n  - openapi/mexc-futures-rest-api-openapi.json\n  - openapi/mexc-spot-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/authentication/mexc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- Finance
- Blockchain
---
