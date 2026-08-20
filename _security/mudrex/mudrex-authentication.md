---
api_key_in:
- header
auth_types:
- apiKey
description: Mudrex runs two independent surfaces with two different auth postures. The public market-data surface (REST klines and the WebSocket stream) is unauthenticated and rate-limited per IP. Every private trading endpoint under /fapi/v1 takes a single API-key header, X-Authentication, carrying the API secret. There is no OAuth, no OIDC, no request signing (no HMAC over the payload), no timestamp/nonce and no scope model — one long-lived bearer secret grants the full trading surface of the account. Issuance is gated on KYC (PAN & Aadhaar) and TOTP two-factor enrollment, and the secret is displayed exactly once at creation.
kind: authentication
layout: security
method: searched
name: Mudrex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mudrex secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mudrex
provider_slug: mudrex
scheme_count: 2
schemes:
- applies_to:
  - mudrex:mudrex-futures-trading-api
  - mudrex:mudrex-mcp-server
  in: header
  name: XAuthentication
  parameter: X-Authentication
  sources:
  - https://docs.trade.mudrex.com/docs/authentication-rate-limits
  type: apiKey
  value: the API secret issued in the Mudrex dashboard
- applies_to:
  - mudrex:mudrex-market-data-api
  detail: GET /fapi/v1/price/kline, GET /fapi/v1/price/mark-kline and wss://trade.mudrex.com/fapi/v1/price/ws/linear are public and read-only.
  name: none
  sources:
  - https://docs.trade.mudrex.com/docs/market-data
  type: public
slug: mudrex-authentication
source_filename: mudrex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  https://docs.trade.mudrex.com/docs/authentication-rate-limits,\n  https://docs.trade.mudrex.com/docs/api-key-management,\n  https://docs.trade.mudrex.com/docs/mcp\ndocs: https://docs.trade.mudrex.com/docs/authentication-rate-limits\ndescription: >-\n  Mudrex runs two independent surfaces with two different auth postures. The\n  public market-data surface (REST klines and the WebSocket stream) is\n  unauthenticated and rate-limited per IP. Every private trading endpoint under\n  /fapi/v1 takes a single API-key header, X-Authentication, carrying the API\n  secret. There is no OAuth, no OIDC, no request signing (no HMAC over the\n  payload), no timestamp/nonce and no scope model — one long-lived bearer\n  secret grants the full trading surface of the account. Issuance is gated on\n  KYC (PAN & Aadhaar) and TOTP two-factor enrollment, and the secret is\n  displayed exactly once at creation.\nsummary:\n  types: [apiKey]\n\
  \  api_key_in: [header]\n  oauth2_flows: []\n  signing: none\n  scopes: none\nschemes:\n- name: XAuthentication\n  type: apiKey\n  in: header\n  parameter: X-Authentication\n  value: the API secret issued in the Mudrex dashboard\n  applies_to:\n  - mudrex:mudrex-futures-trading-api\n  - mudrex:mudrex-mcp-server\n  sources: [https://docs.trade.mudrex.com/docs/authentication-rate-limits]\n- name: none\n  type: public\n  applies_to: [mudrex:mudrex-market-data-api]\n  detail: >-\n    GET /fapi/v1/price/kline, GET /fapi/v1/price/mark-kline and\n    wss://trade.mudrex.com/fapi/v1/price/ws/linear are public and read-only.\n  sources: [https://docs.trade.mudrex.com/docs/market-data]\nissuance:\n  portal: https://mudrex.com/pro-trading\n  prerequisites:\n  - KYC verification (PAN & Aadhaar)\n  - TOTP two-factor authentication enabled on the account\n  secret_shown_once: true\n  management: https://docs.trade.mudrex.com/docs/api-key-management\n  operations: [view, copy, rotate, revoke]\nfailure_modes:\n\
  - status: 401\n  body: '{\"success\": false, \"errors\": [{\"code\": 3100, \"text\": \"Invalid Authentication\"}]}'\n  cause: Missing or invalid X-Authentication header.\n- status: 403\n  cause: Scope / IP not allowed.\n  note: >-\n    The error reference names a 403 \"Scope / IP not allowed\" case, but the docs\n    publish no scope vocabulary and no IP-allowlist configuration page, so the\n    condition that produces it is not documented.\ngaps:\n- No OAuth 2.0 / OIDC and therefore no scopes/ artifact for this provider.\n- No request signing (HMAC), timestamp or nonce — replay protection rests entirely on TLS.\n- No documented key expiry or rotation cadence, and no per-key permission model\n  (read-only vs trade), so an agent integration must be handed a full-trading secret.\n- The same secret authenticates the hosted MCP server, so an MCP client holds\n  full trading authority over the account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mudrex/refs/heads/main/authentication/mudrex-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cryptocurrency
- Trading
- Futures
- Financial-Services
- Fintech
- Market Data
- Exchange
- India
---
