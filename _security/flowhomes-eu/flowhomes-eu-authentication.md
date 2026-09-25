---
anonymous_access: true
api_key_in: []
api_specs:
- filename: flowhomes-eu-openapi.json
  format: json
  label: Qorevia Market Intelligence API
  slug: qorevia-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowhomes-eu/refs/heads/main/openapi/flowhomes-eu-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Flowhomes Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qorevia declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Qorevia
provider_slug: flowhomes-eu
scheme_count: 2
schemes:
- applies_to:
  - session_state
  - risk_levels
  - strategy_grade
  - xau_quote
  - xau_bars
  - xau_market_state
  - csv_profile
  - json_shape
  - jwt_decode
  - tick_pnl
  - evm_address_syntax
  - ohlcv_state
  - regex_test
  challenge:
    body: '{}'
    encoding: base64(JSON)
    header: PAYMENT-REQUIRED
    http_status: 402
    observed: '{x402Version 2, error "Payment required", resource {url, description, mimeType application/json}, accepts[{scheme exact, network eip155:8453, amount "5000", asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, payTo 0x80cdA9077d65Ac1a05454619Bb94B318cf0c3382, maxTimeoutSeconds 300, extra {name "USD Coin", version "2"}}], extensions.bazaar {...}} — GET /api/session-state, 2026-09-19.'
  credential:
    docs_quote: Clients should make the request normally, read the HTTP 402 payment requirements, pay using x402, and retry with PAYMENT-SIGNATURE.
    header: PAYMENT-SIGNATURE
    lifetime: maxTimeoutSeconds 300 from the challenge
    what: an x402 v2 payment payload proving settlement of accepts[].amount in USDC to payTo on eip155:8453, produced by an x402 client, optionally through the facilitator https://facilitator.payai.network
  declared_in_spec: false
  facilitator: https://facilitator.payai.network
  id: x402-payment
  key_prefixes: none (no keys)
  manifest: https://api.flowhomes.eu/.well-known/x402
  optional_headers:
  - name: X-Qorevia-Ref
    purpose: Founders Network referral attribution on a paid call (or the ?ref=QF-... query parameter); not an authenticator
  type: payment (x402 v2) — not an OpenAPI securityScheme type
- applies_to:
  - GET /api/find
  - POST /api/route
  - GET /api/catalog
  - GET /api/try
  - POST /mcp
  - POST /a2a
  - GET /health
  - GET /dashboard
  - GET /api/stats
  - the four qorevia-* beacons
  - /api/magnet*
  - /api/amplifier/stats
  - /api/distribution/stats
  - the /api/club* Founders Network routes
  - /party
  id: none
  note: Anonymous. The club routes identify a caller by a public wallet address supplied in the request (invalid_wallet otherwise); that is an identifier, not a credential.
  type: none
slug: flowhomes-eu-authentication
source_filename: flowhomes-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.flowhomes.eu/skill.md\ndocs: https://api.flowhomes.eu/skill.md\nsummary: >-\n  There is no authentication. openapi/flowhomes-eu-openapi.json declares no securitySchemes and no\n  security requirement (derive-authentication.py correctly produced nothing), and that is accurate: the\n  provider states \"No API key required for paid routes\" (agent card, skill qorevia-x402-seller) and\n  \"There are no accounts\". Access control is PAYMENT: each of the 13 priced operations answers an\n  unpaid request with HTTP 402 and a PAYMENT-REQUIRED header carrying x402 v2 requirements, and serves\n  the response when the same request is retried with a PAYMENT-SIGNATURE header proving a USDC transfer\n  on Base Mainnet. The 21 free routes, the MCP server and the A2A endpoint need nothing at all. No\n  OAuth, OIDC or RFC 9728 metadata is served (all 404 on api.flowhomes.eu, which is also the MCP host).\nschemes:\n- id: x402-payment\n\
  \  type: payment (x402 v2) — not an OpenAPI securityScheme type\n  declared_in_spec: false\n  applies_to: [session_state, risk_levels, strategy_grade, xau_quote, xau_bars, xau_market_state, csv_profile, json_shape, jwt_decode, tick_pnl, evm_address_syntax, ohlcv_state, regex_test]\n  challenge:\n    http_status: 402\n    header: PAYMENT-REQUIRED\n    encoding: base64(JSON)\n    observed: >-\n      {x402Version 2, error \"Payment required\", resource {url, description, mimeType application/json},\n      accepts[{scheme exact, network eip155:8453, amount \"5000\", asset\n      0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, payTo 0x80cdA9077d65Ac1a05454619Bb94B318cf0c3382,\n      maxTimeoutSeconds 300, extra {name \"USD Coin\", version \"2\"}}], extensions.bazaar {...}} — GET\n      /api/session-state, 2026-09-19.\n    body: '{}'\n  credential:\n    header: PAYMENT-SIGNATURE\n    what: an x402 v2 payment payload proving settlement of accepts[].amount in USDC to payTo on eip155:8453, produced\
  \ by an x402 client, optionally through the facilitator https://facilitator.payai.network\n    lifetime: maxTimeoutSeconds 300 from the challenge\n    docs_quote: 'Clients should make the request normally, read the HTTP 402 payment requirements, pay using x402, and retry with PAYMENT-SIGNATURE.'\n  manifest: https://api.flowhomes.eu/.well-known/x402\n  facilitator: https://facilitator.payai.network\n  key_prefixes: none (no keys)\n  optional_headers:\n  - name: X-Qorevia-Ref\n    purpose: 'Founders Network referral attribution on a paid call (or the ?ref=QF-... query parameter); not an authenticator'\n- id: none\n  type: none\n  applies_to: ['GET /api/find', 'POST /api/route', 'GET /api/catalog', 'GET /api/try', 'POST /mcp', 'POST /a2a', 'GET /health', 'GET /dashboard', 'GET /api/stats', 'the four qorevia-* beacons', '/api/magnet*', '/api/amplifier/stats', '/api/distribution/stats', 'the /api/club* Founders Network routes', '/party']\n  note: Anonymous. The club routes identify a caller\
  \ by a public wallet address supplied in the request (invalid_wallet otherwise); that is an identifier, not a credential.\noauth: null\nopenid_connect: null\nmutual_tls: null\napi_keys: null\nmcp_auth:\n  endpoint: https://api.flowhomes.eu/mcp\n  scheme: none — initialize, tools/list and tools/call answered anonymously\n  protected_resource_metadata: 404 (/.well-known/oauth-protected-resource)\n  authorization_server_metadata: 404 (/.well-known/oauth-authorization-server)\na2a_auth:\n  endpoint: https://api.flowhomes.eu/a2a\n  scheme: none — the card declares no securitySchemes; message/send completed anonymously\nsignup: none — no accounts exist; a funded USDC wallet on Base is the only prerequisite\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowhomes-eu/refs/heads/main/authentication/flowhomes-eu-authentication.yml
summary_line: 2 schemes
tags:
- Market Data
- Gold
- XAUUSD
- Trading
- Finance
- Quantitative Research
- Risk Management
- Data Profiling
- Developer Tools
- x402
- USDC
- Base L2
- Agentic Commerce
- pay-per-call
- MCP
- A2A
- Agents
- Agent-Native
---
