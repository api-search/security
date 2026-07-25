---
api_key_in:
- header
api_specs:
- filename: phemex-account-api-openapi.yml
  format: yaml
  label: Phemex Account API
  slug: phemex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-account-api-openapi.yml
- filename: phemex-conversion-api-openapi.yml
  format: yaml
  label: Phemex Conversion API
  slug: phemex-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-conversion-api-openapi.yml
- filename: phemex-market-data-api-openapi.yml
  format: yaml
  label: Phemex Market Data API
  slug: phemex-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-market-data-api-openapi.yml
- filename: phemex-orders-api-openapi.yml
  format: yaml
  label: Phemex Orders API
  slug: phemex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-orders-api-openapi.yml
- filename: phemex-positions-api-openapi.yml
  format: yaml
  label: Phemex Positions API
  slug: phemex-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-positions-api-openapi.yml
- filename: phemex-sub-account-transfers-api-openapi.yml
  format: yaml
  label: Phemex Sub-Account Transfers API
  slug: phemex-sub-account-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-sub-account-transfers-api-openapi.yml
- filename: phemex-trades-api-openapi.yml
  format: yaml
  label: Phemex Trades API
  slug: phemex-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-trades-api-openapi.yml
- filename: phemex-transfers-api-openapi.yml
  format: yaml
  label: Phemex Transfers API
  slug: phemex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-transfers-api-openapi.yml
- filename: phemex-wallets-api-openapi.yml
  format: yaml
  label: Phemex Wallets API
  slug: phemex-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-wallets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phemex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phemex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phemex
provider_slug: phemex
scheme_count: 1
schemes:
- description: HMAC SHA256 signed request. Also requires x-phemex-request-expiry and x-phemex-request-signature headers.
  in: header
  name: HmacAuth
  parameter: x-phemex-access-token
  sources:
  - openapi/contract.yml
  - openapi/hedged-perpetual.yml
  - openapi/spot.yml
  - openapi/transfer.yml
  type: apiKey
slug: phemex-authentication
source_filename: phemex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contract.yml, openapi/hedged-perpetual.yml, openapi/spot.yml, openapi/transfer.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HmacAuth\n  type: apiKey\n  in: header\n  parameter: x-phemex-access-token\n  description: HMAC SHA256 signed request. Also requires x-phemex-request-expiry and x-phemex-request-signature\n    headers.\n  sources:\n  - openapi/contract.yml\n  - openapi/hedged-perpetual.yml\n  - openapi/spot.yml\n  - openapi/transfer.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/authentication/phemex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Derivatives
- Spot Trading
- Perpetual Contracts
- Futures
- WebSocket
- Market Data
---
