---
anonymous_access: false
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hydromancer Leading Hyperliquid Data Provider Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hydromancer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hydromancer
provider_slug: hydromancer-leading-hyperliquid-data-provider
scheme_count: 2
schemes:
- applies_to: Hydromancer REST API (https://api.hydromancer.xyz, POST /info)
  description: 'All REST requests must include an Authorization header carrying the account API key as a Bearer token. A missing or invalid key returns HTTP 401 with body {"error": "Invalid API key"}.'
  format: 'Authorization: Bearer YOUR_API_KEY'
  in: header
  name: rest_bearer_token
  parameter_name: Authorization
  sources:
  - https://docs.hydromancer.xyz/readme/rest-api.md
  type: apiKey
- applies_to: Hydromancer WebSocket API (wss://api.hydromancer.xyz/ws)
  description: The WebSocket API authenticates by passing the same account API key as a query parameter on the connection URL. The exact parameter name is not stated verbatim in the public docs; the key is the same credential used for the REST Bearer token.
  in: query
  name: ws_query_api_key
  parameter_name: null
  sources:
  - https://docs.hydromancer.xyz/readme/websocket.md
  type: apiKey
slug: hydromancer-leading-hyperliquid-data-provider-authentication
source_filename: hydromancer-leading-hyperliquid-data-provider-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://docs.hydromancer.xyz/readme/rest-api.md (REST auth) + https://docs.hydromancer.xyz/readme/get-api-keys.md\ndocs: https://docs.hydromancer.xyz/readme/rest-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  notes: >-\n    Single API-key credential per account. The REST API presents it as an HTTP Bearer token in the\n    Authorization header; the WebSocket API accepts the same key as a query parameter on the connection\n    URL. There is no OAuth, OIDC or mutual-TLS surface. Keys are issued through manual, personalized\n    onboarding (contact data@hydromancer.xyz), not a self-serve dashboard.\nschemes:\n  - name: rest_bearer_token\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    applies_to: Hydromancer REST API (https://api.hydromancer.xyz, POST /info)\n    description: >-\n      All REST requests must include\
  \ an Authorization header carrying the account API key as a Bearer\n      token. A missing or invalid key returns HTTP 401 with body {\"error\": \"Invalid API key\"}.\n    sources: [https://docs.hydromancer.xyz/readme/rest-api.md]\n  - name: ws_query_api_key\n    type: apiKey\n    in: query\n    parameter_name: null\n    applies_to: Hydromancer WebSocket API (wss://api.hydromancer.xyz/ws)\n    description: >-\n      The WebSocket API authenticates by passing the same account API key as a query parameter on the\n      connection URL. The exact parameter name is not stated verbatim in the public docs; the key is\n      the same credential used for the REST Bearer token.\n    sources: [https://docs.hydromancer.xyz/readme/websocket.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydromancer-leading-hyperliquid-data-provider/refs/heads/main/authentication/hydromancer-leading-hyperliquid-data-provider-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Hyperliquid
- Blockchain
- Web3
- DeFi
- Crypto trading data
- Market Data
- Real-Time
- WebSocket streaming
- Historical Data
- Orderbook data
---
