---
api_key_in:
- header
api_specs:
- filename: one-trading-fast-openapi.yml
  format: yaml
  label: One Trading Fast API
  slug: one-trading-fast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/openapi/one-trading-fast-openapi.yml
- filename: one-trading-streams-asyncapi.yml
  format: yaml
  label: One Trading WebSocket Streams API
  slug: one-trading-websocket-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/asyncapi/one-trading-streams-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: One Trading Authentication
name_suffix: Authentication
oauth_flows: []
overview: One Trading secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: One Trading
provider_slug: one-trading
scheme_count: 1
schemes:
- bearerFormat: JWT
  format: 'Authorization: Bearer <token>'
  header: Authorization
  in: header
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/one-trading-fast-openapi.yml
  token_source: API tokens are generated in the One Trading UI. Each token is granted one or more permission scopes at creation time.
  type: http
slug: one-trading-authentication
source_filename: one-trading-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource:\n  - https://docs.onetrading.com/rest/trading/create-order.md\n  - https://docs.onetrading.com/websocket/authenticate.md\n  - https://support.onetrading.com/hc/en-gb/articles/16357722538129\n  - live probes of https://api.onetrading.com/fast/v1\ndocs: https://docs.onetrading.com\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <token>'\n    token_source: >-\n      API tokens are generated in the One Trading UI. Each token is granted one\n      or more permission scopes at creation time.\n    sources: [openapi/one-trading-fast-openapi.yml]\npermissions:\n  model: named-scopes-per-token\n  scopes:\n    - { name: Read, grants: All GET endpoints (account balances, orders, trades, market data) }\n    - { name: Trade,\
  \ grants: Place or cancel orders via POST/DELETE and private WebSocket trading channels }\n    - { name: Withdraw, grants: Deposit and withdraw funds to/from off-site wallets }\n    - { name: SUBACCOUNT_TRANSFER, grants: Transfer balances between the account holder's subaccounts (POST /v1/subaccounts/transfers) }\nwebsocket:\n  url: wss://streams.fast.onetrading.com\n  flow: Send an AUTHENTICATE message with api_token before subscribing to private channels; token must carry the Trade permission.\n  failure_codes: [AUTHENTICATION_FAILED, AUTH_ERROR]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/authentication/one-trading-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Derivatives
- Futures
- Financial Services
- Market Data
- WebSocket
- Fintech
---
