---
api_key_in:
- header
api_specs:
- filename: korbit-websocket-asyncapi.yml
  format: yaml
  label: Korbit Open API v2 WebSocket
  slug: korbit-open-api-v2-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/asyncapi/korbit-websocket-asyncapi.yml
- filename: korbit-asset-api-openapi.yml
  format: yaml
  label: Korbit Asset API
  slug: korbit-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-asset-api-openapi.yml
- filename: korbit-deposit-crypto-api-openapi.yml
  format: yaml
  label: Korbit Deposit (Crypto) API
  slug: korbit-deposit-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-deposit-crypto-api-openapi.yml
- filename: korbit-deposit-withdrawal-krw-api-openapi.yml
  format: yaml
  label: Korbit Deposit/Withdrawal (KRW) API
  slug: korbit-deposit-withdrawal-krw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-deposit-withdrawal-krw-api-openapi.yml
- filename: korbit-other-api-openapi.yml
  format: yaml
  label: Korbit Other API
  slug: korbit-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-other-api-openapi.yml
- filename: korbit-quotation-api-openapi.yml
  format: yaml
  label: Korbit Quotation API
  slug: korbit-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-quotation-api-openapi.yml
- filename: korbit-trading-api-openapi.yml
  format: yaml
  label: Korbit Trading API
  slug: korbit-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-trading-api-openapi.yml
- filename: korbit-withdrawal-crypto-api-openapi.yml
  format: yaml
  label: Korbit Withdrawal (Crypto) API
  slug: korbit-withdrawal-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-withdrawal-crypto-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Korbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Korbit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Korbit
provider_slug: korbit
scheme_count: 1
schemes:
- description: API key issued in the Korbit Developers portal (https://developers.korbit.co.kr). Keys carry permissions (readOrders, writeOrders, readBalances, readDeposits, writeDeposits, readWithdrawals, writeWithdrawals), may be pinned to an IP allowlist, and are valid for one year. Every signed request additionally carries `timestamp` and `signature` parameters (HMAC-SHA256 hex or ED25519 base64).
  in: header
  name: KorbitApiKey
  parameter: X-KAPI-KEY
  sources:
  - openapi/korbit-openapi.yml
  type: apiKey
slug: korbit-authentication
source_filename: korbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/korbit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: KorbitApiKey\n  type: apiKey\n  in: header\n  parameter: X-KAPI-KEY\n  description: API key issued in the Korbit Developers portal (https://developers.korbit.co.kr).\n    Keys carry permissions (readOrders, writeOrders, readBalances, readDeposits, writeDeposits,\n    readWithdrawals, writeWithdrawals), may be pinned to an IP allowlist, and are valid for\n    one year. Every signed request additionally carries `timestamp` and `signature` parameters\n    (HMAC-SHA256 hex or ED25519 base64).\n  sources:\n  - openapi/korbit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/authentication/korbit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Digital Assets
- Trading
- Market Data
- Financial-Services
- WebSocket
- South Korea
- Blockchain
---
