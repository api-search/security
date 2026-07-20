---
api_key_in:
- header
api_specs:
- filename: korbit-openapi.yml
  format: yaml
  label: Korbit Open API v2
  slug: korbit-open-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-openapi.yml
- filename: korbit-websocket-asyncapi.yml
  format: yaml
  label: Korbit Open API v2 WebSocket
  slug: korbit-open-api-v2-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/asyncapi/korbit-websocket-asyncapi.yml
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
- Financial Services
- WebSocket
- South Korea
- Blockchain
---
