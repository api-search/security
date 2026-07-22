---
api_key_in:
- header
api_specs:
- filename: oddpool-feeds-asyncapi.yml
  format: yaml
  label: Oddpool WebSocket Feeds
  slug: oddpool-websocket-feeds
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddpool/refs/heads/main/asyncapi/oddpool-feeds-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Oddpool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oddpool secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oddpool
provider_slug: oddpool
scheme_count: 2
schemes:
- description: REST requests authenticate with an API key passed in the X-API-Key header. Keys are generated from account settings (https://oddpool.com/account) and are prefixed with `oddpool_`. Invalid or expired credentials return 401; a valid key on an insufficient plan tier returns 403.
  in: header
  key_prefix: oddpool_
  name: ApiKeyAuth
  parameter_name: X-API-Key
  sources:
  - https://docs.oddpool.com/authentication.md
  type: apiKey
- description: 'The WebSocket feed (wss://feeds.oddpool.com/ws) authenticates in-band: after connecting, the client sends an auth message {"action":"auth","api_key":"..."} and the server responds with the resolved tier and connection limits.'
  in: message
  name: WebSocketAuth
  parameter_name: api_key
  sources:
  - https://docs.oddpool.com/websocket/overview.md
  type: apiKey
slug: oddpool-authentication
source_filename: oddpool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.oddpool.com/authentication.md\ndocs: https://docs.oddpool.com/authentication.md\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  key_prefix: oddpool_\n  description: >-\n    REST requests authenticate with an API key passed in the X-API-Key header.\n    Keys are generated from account settings (https://oddpool.com/account) and\n    are prefixed with `oddpool_`. Invalid or expired credentials return 401;\n    a valid key on an insufficient plan tier returns 403.\n  sources: [https://docs.oddpool.com/authentication.md]\n- name: WebSocketAuth\n  type: apiKey\n  in: message\n  parameter_name: api_key\n  description: >-\n    The WebSocket feed (wss://feeds.oddpool.com/ws) authenticates in-band: after\n    connecting, the client sends an auth message {\"action\":\"auth\",\"api_key\":\"...\"}\n    and the\
  \ server responds with the resolved tier and connection limits.\n  sources: [https://docs.oddpool.com/websocket/overview.md]\ntiers:\n  note: >-\n    Endpoint groups are gated by subscription plan, not by OAuth scopes. Search\n    and Historical data are Free; WebSocket dist channel is Free, book/trade/\n    snapshot are Pro+; Whale tracking is Pro; Arbitrage and Price spreads are\n    Premium; the Reference Data API is enterprise-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddpool/refs/heads/main/authentication/oddpool-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Prediction Markets
- Market Data
- Financial Data
- Trading
- Fintech
- Data Aggregation
- WebSocket
- Historical Data
- Kalshi
- Polymarket
---
