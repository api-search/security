---
api_key_in:
- header
api_specs:
- filename: totalis-openapi-original.json
  format: json
  label: Totalis RFQ API
  slug: totalis-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/totalis/refs/heads/main/openapi/totalis-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Totalis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Totalis secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Totalis
provider_slug: totalis
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Privy JWT issued to the web dashboard. Sent as `Authorization: Bearer <jwt>`. The Privy session signer underpins all wallet-signed actions.'
  name: PrivyJWT
  scheme: bearer
  sources:
  - openapi/totalis-openapi-original.json
  type: http
- description: 'Programmatic API key. Sent as `X-API-Key: <key>`. Generate one from the Totalis dashboard (app.totalis.trade, account settings). The full key is shown only at creation. The same header is accepted on the WebSocket auth message ({"type": "auth", "api_key": "<key>"}).'
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/totalis-openapi-original.json
  type: apiKey
slug: totalis-authentication
source_filename: totalis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.totalis.trade/guides/authentication\ndocs: https://docs.totalis.trade/guides/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Two schemes, accepted interchangeably on every authenticated endpoint: a\n    scoped programmatic API key (X-API-Key header, also accepted on the\n    WebSocket auth message) and a Privy JWT bearer token used by the web\n    dashboard. The one exception is POST /v1/api-keys (create key), which\n    requires a Privy JWT or a key holding the keys:manage scope. A new key can\n    never grant a scope the creating credential does not already hold.\nschemes:\n- name: PrivyJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Privy JWT issued to the web dashboard. Sent as `Authorization: Bearer <jwt>`.\n    The Privy session signer underpins all wallet-signed actions.'\n  sources:\n  - openapi/totalis-openapi-original.json\n\
  - name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Programmatic API key. Sent as `X-API-Key: <key>`. Generate one from the Totalis\n    dashboard (app.totalis.trade, account settings). The full key is shown only at creation.\n    The same header is accepted on the WebSocket auth message\n    ({\"type\": \"auth\", \"api_key\": \"<key>\"}).'\n  sources:\n  - openapi/totalis-openapi-original.json\nkey_scopes:\n  description: >-\n    Every API key carries a set of scopes chosen at creation. A request to an\n    endpoint whose scope the key lacks is rejected with 403 (insufficient_scope).\n    Webhook deliveries are also gated on the key's scopes, re-checked at delivery\n    time.\n  docs: https://docs.totalis.trade/guides/authentication#scopes\n  scopes:\n  - scope: account:read\n    grants: View account profile and username.\n    risk: low\n  - scope: markets:read\n    grants: Browse markets and exclusion groups.\n    risk: low\n  - scope: positions:read\n\
  \    grants: View quote requests, portfolio, stats, and P&L.\n    risk: low\n  - scope: balances:read\n    grants: View wallet and vault balances and delegation status.\n    risk: low\n  - scope: trading:write\n    grants: Create, modify, commit, and cancel quote requests (place parlays).\n    risk: medium\n  - scope: funds:deposit\n    grants: Move USDC into the vault.\n    risk: low\n  - scope: funds:withdraw\n    grants: Move USDC out of the vault/wallet to any address. Can drain the account.\n    risk: high\n  - scope: account:write\n    grants: Change username and profile settings.\n    risk: medium\n  - scope: tx:sign\n    grants: Submit arbitrary signed Solana transactions.\n    risk: high\n  - scope: keys:manage\n    grants: Create, list, and revoke API keys. Lets a key mint more keys.\n    risk: high\n  - scope: mm:quote\n    grants: Read RFQs and submit/confirm quotes as a market maker.\n    risk: medium\nkey_lifecycle:\n  states: [active, revoked, expired]\n  management:\n \
  \   list: GET /v1/api-keys\n    create: POST /v1/api-keys (Privy JWT or keys:manage scope required)\n    revoke: DELETE /v1/api-keys/{prefix}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totalis/refs/heads/main/authentication/totalis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Prediction Markets
- Derivatives
- Parlays
- Trading
- RFQ
- Solana
- Crypto Web3
- Market Data
- Webhooks
---
