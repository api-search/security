---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Financialdata Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinancialData.Net declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FinancialData.Net
provider_slug: financialdata-net
scheme_count: 1
schemes:
- applies_to:
  - REST API (https://financialdata.net/api/v1/*)
  - MCP server (https://financialdata.net/mcp?key=API_KEY)
  - Python SDK (FinancialDataClient(api_key=...))
  - Excel add-in (key saved in the task pane)
  description: Account API key appended to every request URL as ?key=API_KEY (or &key=API_KEY when other query parameters are already present). Obtained from the account dashboard after sign-in.
  id: api_key_query
  in: query
  name: key
  required: true
  type: apiKey
slug: financialdata-net-authentication
source_filename: financialdata-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://financialdata.net/documentation (Introduction), https://financialdata.net/faq, https://financialdata.net/mcp-server, live probes of https://financialdata.net/api/v1/stock-symbols\ndocs: https://financialdata.net/documentation\nnote: >-\n  Single-scheme API. There is no OpenAPI to derive securitySchemes from, so this profile is read\n  from the provider's own documentation and confirmed against live probes. The API key is a\n  QUERY-STRING parameter, not a header — the docs say \"ensure that each URL ends with ?key=API_KEY.\n  If the URL already contains other query parameters, use &key=API_KEY\". The same key authenticates\n  the REST API, the Python SDK, the Excel add-in and the hosted MCP server. Keys are issued from the\n  signed-in account dashboard; there is no OAuth, no OIDC, no mTLS, no signed requests, and no\n  documented key rotation, expiry, scoping or per-key restriction. /.well-known/openid-configuration,\n\
  \  /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource all return 404.\n  Because the credential rides in the URL it is exposed to proxy logs, browser history, referrer\n  headers and CDN access logs — worth flagging to any agent that constructs request URLs from\n  templates or logs them.\nschemes:\n  - id: api_key_query\n    type: apiKey\n    in: query\n    name: key\n    description: >-\n      Account API key appended to every request URL as ?key=API_KEY (or &key=API_KEY when other\n      query parameters are already present). Obtained from the account dashboard after sign-in.\n    required: true\n    applies_to:\n      - REST API (https://financialdata.net/api/v1/*)\n      - MCP server (https://financialdata.net/mcp?key=API_KEY)\n      - Python SDK (FinancialDataClient(api_key=...))\n      - Excel add-in (key saved in the task pane)\noauth2: false\nopenid_connect: false\nmutual_tls: false\nsigned_requests: false\nkey_management:\n  issuance: Account dashboard\
  \ at https://financialdata.net after sign-in\n  rotation_documented: false\n  expiry_documented: false\n  scoping_documented: false\n  multiple_keys_documented: false\n  ip_allowlist_documented: false\nobserved:\n  - probe: GET https://financialdata.net/api/v1/stock-symbols\n    status: 401\n    body: '{\"message\": \"Invalid API key\"}'\n    note: No key supplied.\n  - probe: GET https://financialdata.net/api/v1/stock-symbols?key=<invalid>\n    status: 401\n    body: '{\"message\": \"Invalid API key\"}'\n    note: Same envelope for a malformed key — no distinction between missing and invalid.\n  - probe: 'POST https://financialdata.net/mcp {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n    status: 200\n    body: '{\"jsonrpc\":\"2.0\",\"id\":null,\"error\":{\"code\":-32001,\"message\":\"Unauthorized\"}}'\n    note: MCP returns HTTP 200 with a JSON-RPC error rather than a 401, per the JSON-RPC convention.\nplan_gating: >-\n  Authentication succeeds or fails on the key alone;\
  \ the PLAN attached to the key then decides which\n  of the 86 endpoints answer. 9 endpoints are on Free, 43 cumulative on Standard, all 86 on Premium\n  and above; the MCP server additionally requires Professional or Enterprise.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financialdata-net/refs/heads/main/authentication/financialdata-net-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Financial Data
- stock-market-api
- Market Data
- Equities
- ETFs
- Crypto
- Forex
- derivatives-options
- Fundamentals
- Insider Trading
- institutional-13f
- ESG
- Economic Data
- MCP
- Investing
- Trading
---
