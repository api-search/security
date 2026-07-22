---
api_key_in:
- header
api_specs:
- filename: loot-rush-games-partner-openapi.json
  format: json
  label: LootRush Partner API
  slug: lootrush-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loot-rush-games/refs/heads/main/openapi/loot-rush-games-partner-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Loot Rush Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loot Rush Games secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loot Rush Games
provider_slug: loot-rush-games
scheme_count: 2
schemes:
- description: 'API token issued by your LootRush account manager. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/loot-rush-games-partner-openapi.json
  type: http
- description: Integration API key provided by LootRush during Connect registration.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/loot-rush-games-partner-openapi.json
  type: apiKey
slug: loot-rush-games-authentication
source_filename: loot-rush-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/loot-rush-games-partner-openapi.json\ndocs: https://docs.lootrush.com/\nnotes: >-\n  Withdraw, History and MCP surfaces use Bearer token auth (account API key from\n  Settings -> API Key). Connect uses the x-api-key integration key issued during\n  Connect registration. The MCP surface additionally enforces key scopes (`mcp`,\n  `mcp_card_reveal`). No OAuth2 scheme is declared.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued by your LootRush account manager. Sent as `Authorization: Bearer\n    <token>`.'\n  sources:\n  - openapi/loot-rush-games-partner-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Integration API key provided by LootRush during Connect registration.\n  sources:\n  - openapi/loot-rush-games-partner-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loot-rush-games/refs/heads/main/authentication/loot-rush-games-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cryptocurrency
- Blockchain
- Gaming
- Fintech
- Wallets
- Cards
- Payments
- Withdrawals
- MCP
- Agent-Ready
---
