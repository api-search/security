---
api_key_in:
- header
api_specs:
- filename: rho-protocol-openapi-original.json
  format: json
  label: Rho Exchange API
  slug: rho-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rho-protocol/refs/heads/main/openapi/rho-protocol-openapi-original.json
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Rho Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rho Protocol secures its APIs with apiKey and http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rho Protocol
provider_slug: rho-protocol
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/rho-protocol-openapi-original.json
  type: apiKey
slug: rho-protocol-authentication
source_filename: rho-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rho-protocol-openapi-original.json\ndocs: https://docs.rho.trading/api-reference/authentication.md\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Rho X (rho.trading) uses wallet-signature session auth plus long-lived API keys.\n    There is no OAuth2 authorization server; credentials are minted via the Auth API\n    after signing an Ethereum wallet nonce, or issued as scoped API keys.\ncredentials:\n- name: Access token (Bearer)\n  transport: 'Authorization: Bearer <accessToken>'\n  issued_by: POST /auth-api/v1/login (after signing a nonce from POST /auth-api/v1/nonce with an Ethereum wallet)\n  ttl: Sliding 7 days, resets on each successful call\n  scope: FullAccess\n  use: User-scoped session access\n- name: API key\n  transport: 'Authorization: <apiKey>'\n  issued_by: Rho X interface or POST /apikeys (optional expiresAt)\n  ttl: Long-lived until rotated\
  \ or optional expiresAt\n  scopes:\n  - ReadOnly\n  - FullAccess\n  use: Backend services, trading bots, automation\n- name: WS session token\n  transport: WebSocket authenticate message\n  issued_by: POST /auth-api/v1/ws-session (requires Bearer or ApiKey auth; rate-limit weight 3)\n  ttl: 1 hour by default, refreshable\n  use: Authenticated WebSocket private-channel subscriptions on wss://stream.x.rho.trading/ws-api/v1\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/rho-protocol-openapi-original.json\nauth_api:\n  base_url: https://api.x.rho.trading/auth-api/v1\n  endpoints:\n  - {path: /nonce, method: POST, desc: Request a nonce to sign with the wallet}\n  - {path: /login, method: POST, desc: Exchange signed nonce for an access token (FullAccess)}\n  - {path: /apikeys, method: POST, desc: 'Create an API key (label, scopes, optional expiresAt)'}\n  - {path: /apikeys, method: GET, desc: List active API keys}\n  - {path: /apikeys/revoke,\
  \ method: POST, desc: Revoke an API key}\n  - {path: /ws-session, method: POST, desc: Create a WS session token}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rho-protocol/refs/heads/main/authentication/rho-protocol-authentication.yml
summary_line: apiKey/http-bearer · 1 scheme
tags:
- Company
- Trading
- DeFi
- Derivatives
- Capital Markets
- Blockchain
- Market Data
- WebSocket
- MCP
---
