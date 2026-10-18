---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bigone-account-api-openapi.yml
  format: yaml
  label: BigONE Account API
  slug: bigone-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-account-api-openapi.yml
- filename: bigone-asset-api-openapi.yml
  format: yaml
  label: BigONE Asset API
  slug: bigone-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-asset-api-openapi.yml
- filename: bigone-assets-api-openapi.yml
  format: yaml
  label: BigONE Assets API
  slug: bigone-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-assets-api-openapi.yml
- filename: bigone-deposit-api-openapi.yml
  format: yaml
  label: BigONE Deposit API
  slug: bigone-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-deposit-api-openapi.yml
- filename: bigone-funding-account-api-openapi.yml
  format: yaml
  label: BigONE Funding Account API
  slug: bigone-funding-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-funding-account-api-openapi.yml
- filename: bigone-market-data-api-openapi.yml
  format: yaml
  label: BigONE Market Data API
  slug: bigone-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-market-data-api-openapi.yml
- filename: bigone-order-api-openapi.yml
  format: yaml
  label: BigONE Order API
  slug: bigone-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-order-api-openapi.yml
- filename: bigone-ping-api-openapi.yml
  format: yaml
  label: BigONE Ping API
  slug: bigone-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ping-api-openapi.yml
- filename: bigone-position-api-openapi.yml
  format: yaml
  label: BigONE Position API
  slug: bigone-position-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-position-api-openapi.yml
- filename: bigone-quote-api-openapi.yml
  format: yaml
  label: BigONE Quote API
  slug: bigone-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-quote-api-openapi.yml
- filename: bigone-ranges-api-openapi.yml
  format: yaml
  label: BigONE Ranges API
  slug: bigone-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ranges-api-openapi.yml
- filename: bigone-trade-api-openapi.yml
  format: yaml
  label: BigONE Trade API
  slug: bigone-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trade-api-openapi.yml
- filename: bigone-trades-api-openapi.yml
  format: yaml
  label: BigONE Trades API
  slug: bigone-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trades-api-openapi.yml
- filename: bigone-transfer-api-openapi.yml
  format: yaml
  label: BigONE Transfer API
  slug: bigone-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-transfer-api-openapi.yml
- filename: bigone-withdrawal-api-openapi.yml
  format: yaml
  label: BigONE Withdrawal API
  slug: bigone-withdrawal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-withdrawal-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bigone Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigONE secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BigONE
provider_slug: bigone
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Client-signed JWT (HS256) sent as Authorization: Bearer <token>. Payload claims: type "OpenAPIV2" (required), sub = API Key (required), nonce = timestamp in nanoseconds (required), recv_window = allowable offset in seconds (optional, default 30). Signed with the API Secret as-is (not Base64 encoded).'
  key_management: https://open.big.one/docs/api-key-setup
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bigone-contract-openapi.yml
  - openapi/bigone-convert-openapi.yml
  - openapi/bigone-spot-openapi.yml
  - openapi/bigone-wallet-openapi.yml
  type: http
  websocket: Spot WebSocket authenticates in-message; Contract private stream passes the JWT in the Authorization header of the handshake.
slug: bigone-authentication
source_filename: bigone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://open.big.one/docs/authentication (upgraded from the bearerAuth scheme\n  in the four OpenAPI files)\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/bigone-contract-openapi.yml\n  - openapi/bigone-convert-openapi.yml\n  - openapi/bigone-spot-openapi.yml\n  - openapi/bigone-wallet-openapi.yml\n  description: 'Client-signed JWT (HS256) sent as Authorization: Bearer <token>. Payload\n    claims: type \"OpenAPIV2\" (required), sub = API Key (required), nonce = timestamp\n    in nanoseconds (required), recv_window = allowable offset in seconds (optional,\n    default 30). Signed with the API Secret as-is (not Base64 encoded).'\n  key_management: https://open.big.one/docs/api-key-setup\n  websocket: Spot WebSocket authenticates in-message; Contract private stream passes\n    the JWT in the Authorization header of the handshake.\ndocs:\
  \ https://open.big.one/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/authentication/bigone-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- Wallets
- Market Data
---
