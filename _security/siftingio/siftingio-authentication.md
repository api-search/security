---
api_key_in:
- header
- query
api_specs:
- filename: siftingio-asyncapi.yaml
  format: yaml
  label: SiftingIO Live Stream
  slug: siftingio-live-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/asyncapi/siftingio-asyncapi.yaml
- filename: siftingio-commodities-api-openapi.yml
  format: yaml
  label: SiftingIO Commodities API
  slug: siftingio-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-commodities-api-openapi.yml
- filename: siftingio-convert-api-openapi.yml
  format: yaml
  label: SiftingIO Convert API
  slug: siftingio-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-convert-api-openapi.yml
- filename: siftingio-crypto-api-openapi.yml
  format: yaml
  label: SiftingIO Crypto API
  slug: siftingio-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-crypto-api-openapi.yml
- filename: siftingio-dex-api-openapi.yml
  format: yaml
  label: SiftingIO DEX API
  slug: siftingio-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-dex-api-openapi.yml
- filename: siftingio-economiccalendar-api-openapi.yml
  format: yaml
  label: SiftingIO Economic Calendar API
  slug: siftingio-economiccalendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-economiccalendar-api-openapi.yml
- filename: siftingio-filers-api-openapi.yml
  format: yaml
  label: SiftingIO Filers API
  slug: siftingio-filers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-filers-api-openapi.yml
- filename: siftingio-forex-api-openapi.yml
  format: yaml
  label: SiftingIO Forex API
  slug: siftingio-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-forex-api-openapi.yml
- filename: siftingio-live-api-openapi.yml
  format: yaml
  label: SiftingIO Live API
  slug: siftingio-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-live-api-openapi.yml
- filename: siftingio-markets-api-openapi.yml
  format: yaml
  label: SiftingIO Markets API
  slug: siftingio-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-markets-api-openapi.yml
- filename: siftingio-signals-api-openapi.yml
  format: yaml
  label: SiftingIO Signals API
  slug: siftingio-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-signals-api-openapi.yml
- filename: siftingio-stocks-api-openapi.yml
  format: yaml
  label: SiftingIO Stocks API
  slug: siftingio-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-stocks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Siftingio Authentication
name_suffix: Authentication
oauth_flows: []
overview: SiftingIO secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SiftingIO
provider_slug: siftingio
scheme_count: 3
schemes:
- applies_to: all 37 REST operations (declared in top-level security[])
  example: 'X-API-Key: sft_•••'
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  preference_reason: '"query strings can leak in logs" — https://sifting.io/docs/quickstart'
  preferred: true
  sources:
  - openapi/siftingio-commodities-api-openapi.yml
  - openapi/siftingio-convert-api-openapi.yml
  - openapi/siftingio-crypto-api-openapi.yml
  - openapi/siftingio-dex-api-openapi.yml
  - openapi/siftingio-economiccalendar-api-openapi.yml
  - openapi/siftingio-filers-api-openapi.yml
  - openapi/siftingio-forex-api-openapi.yml
  - openapi/siftingio-live-api-openapi.yml
  - openapi/siftingio-markets-api-openapi.yml
  - openapi/siftingio-signals-api-openapi.yml
  - openapi/siftingio-stocks-api-openapi.yml
  type: apiKey
- applies_to: all 37 REST operations
  example: ?api_key=sft_•••
  in: query
  name: ApiKeyQuery
  parameter: api_key
  preferred: false
  sources:
  - openapi/siftingio-commodities-api-openapi.yml
  - openapi/siftingio-convert-api-openapi.yml
  - openapi/siftingio-crypto-api-openapi.yml
  - openapi/siftingio-dex-api-openapi.yml
  - openapi/siftingio-economiccalendar-api-openapi.yml
  - openapi/siftingio-filers-api-openapi.yml
  - openapi/siftingio-forex-api-openapi.yml
  - openapi/siftingio-live-api-openapi.yml
  - openapi/siftingio-markets-api-openapi.yml
  - openapi/siftingio-signals-api-openapi.yml
  - openapi/siftingio-stocks-api-openapi.yml
  status: accepted fallback
  type: apiKey
- endpoint: wss://stream.sifting.io/ws/v1
  example: wss://stream.sifting.io/ws/v1?key=sft_•••
  exclusive: true
  exclusive_note: 'The only WebSocket auth method. From the AsyncAPI info.description: "the API key is passed as the `key` query parameter (the only WebSocket auth method)". The quickstart gives the reason: browsers cannot set custom headers on the WS handshake.'
  in: query
  in_openapi: false
  name: WebSocketKeyQuery
  parameter: key
  sources:
  - asyncapi/siftingio-asyncapi.yaml
  - https://sifting.io/docs/quickstart
  transport: wss
  type: apiKey
slug: siftingio-authentication
source_filename: siftingio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\ndocs: https://sifting.io/docs/quickstart\nsource: >-\n  https://sifting.io/docs/quickstart (step 02, \"API key & headers\") upgrading the derived baseline\n  from openapi/_original/siftingio-openapi.yaml (components.securitySchemes) and\n  asyncapi/siftingio-asyncapi.yaml\nnote: >-\n  Upgraded from derived to searched. The OpenAPI declares only the two REST schemes; the docs add\n  three facts the spec cannot express — the `sft_` key prefix, the WebSocket `?key=` query\n  parameter (the ONLY WebSocket auth method, because browsers cannot set headers on a WS\n  handshake), and the provider's own preference order (header over query, \"query strings can\n  leak in logs\"). The AsyncAPI document confirms the WebSocket method independently.\n\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oidc: false\n  mtls: false\n  basic: false\n  bearer: false\n  model: single long-lived API key, one key across REST\
  \ + WebSocket + FIX + all three SDKs\n  key_prefix: sft_\n  scoped_keys: true\n  scoped_keys_note: '\"Scoped API keys\" from Builder tier up; \"scoped API keys per environment\" on Enterprise.'\n  rotation_docs: null\n  rotation_note: 'Key generation is in the dashboard (https://sifting.io/dashboard); no public rotation/expiry policy is documented.'\n\nschemes:\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    preferred: true\n    preference_reason: '\"query strings can leak in logs\" — https://sifting.io/docs/quickstart'\n    example: 'X-API-Key: sft_•••'\n    applies_to: all 37 REST operations (declared in top-level security[])\n    sources:\n      - openapi/siftingio-commodities-api-openapi.yml\n      - openapi/siftingio-convert-api-openapi.yml\n      - openapi/siftingio-crypto-api-openapi.yml\n      - openapi/siftingio-dex-api-openapi.yml\n      - openapi/siftingio-economiccalendar-api-openapi.yml\n      - openapi/siftingio-filers-api-openapi.yml\n\
  \      - openapi/siftingio-forex-api-openapi.yml\n      - openapi/siftingio-live-api-openapi.yml\n      - openapi/siftingio-markets-api-openapi.yml\n      - openapi/siftingio-signals-api-openapi.yml\n      - openapi/siftingio-stocks-api-openapi.yml\n  - name: ApiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    preferred: false\n    status: accepted fallback\n    example: '?api_key=sft_•••'\n    applies_to: all 37 REST operations\n    sources:\n      - openapi/siftingio-commodities-api-openapi.yml\n      - openapi/siftingio-convert-api-openapi.yml\n      - openapi/siftingio-crypto-api-openapi.yml\n      - openapi/siftingio-dex-api-openapi.yml\n      - openapi/siftingio-economiccalendar-api-openapi.yml\n      - openapi/siftingio-filers-api-openapi.yml\n      - openapi/siftingio-forex-api-openapi.yml\n      - openapi/siftingio-live-api-openapi.yml\n      - openapi/siftingio-markets-api-openapi.yml\n      - openapi/siftingio-signals-api-openapi.yml\n      - openapi/siftingio-stocks-api-openapi.yml\n\
  \  - name: WebSocketKeyQuery\n    type: apiKey\n    in: query\n    parameter: key\n    transport: wss\n    endpoint: wss://stream.sifting.io/ws/v1\n    example: 'wss://stream.sifting.io/ws/v1?key=sft_•••'\n    exclusive: true\n    exclusive_note: >-\n      The only WebSocket auth method. From the AsyncAPI info.description: \"the API key is passed\n      as the `key` query parameter (the only WebSocket auth method)\". The quickstart gives the\n      reason: browsers cannot set custom headers on the WS handshake.\n    sources: [asyncapi/siftingio-asyncapi.yaml, 'https://sifting.io/docs/quickstart']\n    in_openapi: false\n\nsurfaces:\n  rest:\n    base_url: https://api.sifting.io\n    methods: [X-API-Key header, api_key query param]\n    gate_behaviour: >-\n      Enforced on EVERY /v1/* path before routing. Verified live: GET /v1/openapi.json returns\n      401 {\"error\":\"missing api key (X-API-Key header or api_key query param)\"} and a nonsense\n      path GET /v1/definitely-not-a-real-path-zzz\
  \ with a bad key returns the identical\n      401 {\"error\":\"invalid api key\"}. A 401 from this host therefore says nothing about whether\n      the path exists.\n  websocket:\n    base_url: wss://stream.sifting.io/ws/v1\n    methods: [key query param]\n  fix:\n    docs: https://sifting.io/docs/fix-api\n    methods: [FIX 4.4 session credentials]\n    note: 'Session configuration and feed tiers documented in prose only; no machine-readable contract.'\n  mcp:\n    method: SIFTING_API_KEY environment variable\n    note: >-\n      The MCP server runs locally and reads the same key from the environment. It is not an\n      OAuth-protected remote server — there is no remote server. See mcp/siftingio-mcp.yml.\n\nerrors:\n  - {status: 401, code: unauthorized, meaning: API key missing or invalid, retryable: false}\n  - {status: 403, code: null, meaning: 'Valid key, but the plan or tier does not include this market/venue — entitlement, not authentication', retryable: false}\nentitlement_note:\
  \ >-\n  The 401/403 split matters for an agent: 401 is a credential problem and must not be retried;\n  403 is a PER-MARKET subscription boundary (a Crypto key cannot read Commodities) and must not be\n  retried either, but the remedy is commercial, not technical. See\n  plans/siftingio-plans-pricing.yml.\n\naccount_level_auth:\n  note: >-\n    Distinct from API authentication. SSO and SAML 2.0, SCIM provisioning (where available) and\n    RBAC are offered for DASHBOARD access on Enterprise plans per https://sifting.io/llms.txt.\n    These govern who can log in and mint keys, not how an API call is authenticated. No OIDC or\n    OAuth discovery document is served — /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server returned 404 on all three hosts.\n\nsignup: https://sifting.io/register\nlogin: https://sifting.io/login\ndashboard: https://sifting.io/dashboard\nfree_key: 'Free tier per market, no card required — 10,000 REST calls/mo, 60 req/min, 1 month of\
  \ history.'\nscopes_artifact: null\nscopes_note: >-\n  No scopes/ artifact: the API has no OAuth surface, so there are no scopes to enumerate.\n  Entitlement is expressed as per-market subscription tiers, not token scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/authentication/siftingio-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Financial market data
- Stocks/equities
- Forex
- Cryptocurrency
- DeFi/on-chain
- Commodities
- SEC filings
- XBRL
- Fundamentals
- Fintech
- Quant/trading infrastructure
- Real-time streaming
- WebSocket
- FIX
- financial data
- Market Data
- stocks
- DeFi
- Real-Time
- REST API
- MCP server
- agent-native
---
