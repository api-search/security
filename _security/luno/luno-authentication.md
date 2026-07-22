---
api_key_in: []
api_specs:
- filename: luno-streaming-asyncapi.yml
  format: yaml
  label: Luno API
  slug: luno-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/luno/refs/heads/main/asyncapi/luno-streaming-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Luno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luno
provider_slug: luno
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The API Key ID is sent as the username and the API Key Secret as the password. API keys are created in the Luno account settings and can be scoped with per-key permissions (e.g. Perm_R_Balance, Perm_W_Orders, Perm_W_Send, Perm_W_Withdrawals). Unauthenticated calls to private endpoints return HTTP 401.
  docs: https://www.luno.com/developers/api
  name: apiKeyPair
  scheme: basic
  type: http
slug: luno-authentication
source_filename: luno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.luno.com/developers/api + live 401 probe\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: apiKeyPair\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. The API Key ID is sent as the username and the\n      API Key Secret as the password. API keys are created in the Luno account\n      settings and can be scoped with per-key permissions (e.g. Perm_R_Balance,\n      Perm_W_Orders, Perm_W_Send, Perm_W_Withdrawals). Unauthenticated calls to\n      private endpoints return HTTP 401.\n    docs: https://www.luno.com/developers/api\nnotes: >-\n  Public market-data endpoints (tickers, ticker, orderbook, trades, markets,\n  candles) require no authentication. All account, trading, transfer, send and\n  withdrawal endpoints require the API key pair. There is no OAuth surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luno/refs/heads/main/authentication/luno-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Bitcoin
- Ethereum
- Trading
- Fintech
- Wallet
- Blockchain
- Financial Services
---
