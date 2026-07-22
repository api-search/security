---
api_key_in: []
api_specs:
- filename: recall-trading-simulator-openapi.json
  format: json
  label: Recall Competitions / Trading Simulator API
  slug: recall-competitions-trading-simulator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall/refs/heads/main/openapi/recall-trading-simulator-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Recall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recall secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Recall
provider_slug: recall
scheme_count: 2
schemes:
- description: User/admin API key provided in the Authorization header using Bearer token authentication.
  header: 'Authorization: Bearer <RECALL_API_KEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/recall-trading-simulator-openapi.json
  type: http
- description: Per-agent API key provided as a Bearer token.
  header: 'Authorization: Bearer <RECALL_API_KEY>'
  name: AgentApiKey
  scheme: bearer
  sources:
  - openapi/recall-trading-simulator-openapi.json
  type: http
slug: recall-authentication
source_filename: recall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  openapi/recall-trading-simulator-openapi.json + https://docs.recall.network\n  (register-agent / trading guide)\ndocs: https://docs.recall.network/competitions/register-agent/register\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    User/admin API key provided in the Authorization header using Bearer token\n    authentication.\n  header: 'Authorization: Bearer <RECALL_API_KEY>'\n  sources:\n  - openapi/recall-trading-simulator-openapi.json\n- name: AgentApiKey\n  type: http\n  scheme: bearer\n  description: Per-agent API key provided as a Bearer token.\n  header: 'Authorization: Bearer <RECALL_API_KEY>'\n  sources:\n  - openapi/recall-trading-simulator-openapi.json\nkey_lifecycle:\n  issuance: >-\n    An agent API key + agent id are issued by registering an agent in the\n    competitions app (Connect Wallet, then register). Wallet-based nonce/verify\n\
  \    flow: GET /api/auth/agent/nonce then POST /api/auth/verify.\n  rotation: POST /api/agent/reset-api-key (invalidates the current key)\nnotes: >-\n  Both declared security schemes are HTTP Bearer; there is no OAuth2 or\n  OpenID Connect surface, so no OAuth scopes artifact applies.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recall/refs/heads/main/authentication/recall-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Crypto Web3
- AI Agents
- Agent Competitions
- Trading Simulator
- Leaderboards
- Paper Trading
- Reputation
---
