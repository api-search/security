---
api_key_in:
- header
- query
api_specs:
- filename: infoway-real-time-market-data-api-streaming-asyncapi.yml
  format: yaml
  label: Infoway WebSocket Streaming API
  slug: infoway-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/asyncapi/infoway-real-time-market-data-api-streaming-asyncapi.yml
- filename: infoway-real-time-market-data-api-common-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Common API
  slug: infoway-real-time-market-data-api-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-common-api-openapi.yml
- filename: infoway-real-time-market-data-api-crypto-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Crypto API
  slug: infoway-real-time-market-data-api-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-crypto-api-openapi.yml
- filename: infoway-real-time-market-data-api-stock-api-openapi.yml
  format: yaml
  label: Infoway Real-time Market Data API Stock API
  slug: infoway-real-time-market-data-api-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/openapi/infoway-real-time-market-data-api-stock-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Infoway Real Time Market Data Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infoway Real-time Market Data API secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infoway Real-time Market Data API
provider_slug: infoway-real-time-market-data-api
scheme_count: 3
schemes:
- applied_to: all 13 published operations
  in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/infoway-real-time-market-data-api-openapi.yml
  surface: rest
  type: apiKey
- derived: true
  in: query
  name: WebSocketApiKey
  note: 'Supplied on the connection URL: wss://data.infoway.io/ws?business={stock|crypto|common}&apikey=KEY. Case differs from the REST header (apikey vs apiKey) — a real integration trap. Carrying the key in a query string also means it can land in proxy and server logs.'
  parameter: apikey
  sources:
  - https://infoway.readme.io/reference/ws-subscription.md
  surface: websocket
  type: apiKey
- derived: true
  in: env
  name: MCPServerKey
  note: The stdio MCP server reads the same key from the environment and forwards it via the SDK.
  parameter: INFOWAY_API_KEY
  sources:
  - https://docs.infoway.io/sdk-and-tools/mcp-server.md
  - https://raw.githubusercontent.com/infoway-api/infoway-mcp-server/HEAD/SKILL.md
  surface: mcp
  type: apiKey
slug: infoway-real-time-market-data-api-authentication
source_filename: infoway-real-time-market-data-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/infoway-real-time-market-data-api-openapi.yml\ndocs: https://infoway.readme.io/reference/api-key-application\ndocs_additional:\n  - https://infoway.readme.io/reference/api-protocols-and-response-formats.md\n  - https://infoway.readme.io/reference/ws-subscription.md\n  - https://docs.infoway.io/sdk-and-tools/mcp-server.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  scopes: false\n  note: >-\n    Single-factor API-key authentication across every surface. No OAuth, no OpenID Connect, no bearer\n    tokens, no mTLS, no scopes and no token exchange. The key is the whole authorization model — plan\n    entitlements are attached to the key server-side.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  surface: rest\n  sources:\n  - openapi/infoway-real-time-market-data-api-openapi.yml\n  applied_to: all 13 published operations\n- name: WebSocketApiKey\n\
  \  type: apiKey\n  in: query\n  parameter: apikey\n  surface: websocket\n  sources:\n  - https://infoway.readme.io/reference/ws-subscription.md\n  note: >-\n    Supplied on the connection URL: wss://data.infoway.io/ws?business={stock|crypto|common}&apikey=KEY.\n    Case differs from the REST header (apikey vs apiKey) — a real integration trap. Carrying the key in a\n    query string also means it can land in proxy and server logs.\n  derived: true\n- name: MCPServerKey\n  type: apiKey\n  in: env\n  parameter: INFOWAY_API_KEY\n  surface: mcp\n  sources:\n  - https://docs.infoway.io/sdk-and-tools/mcp-server.md\n  - https://raw.githubusercontent.com/infoway-api/infoway-mcp-server/HEAD/SKILL.md\n  note: The stdio MCP server reads the same key from the environment and forwards it via the SDK.\n  derived: true\nkey_management:\n  issuance: >-\n    Register at https://infoway.io/en/create-account, then the key is issued from the dashboard at\n    https://infoway.io/dashboard.\n  one_key_per_plan:\
  \ true\n  multiple_plans_per_account: true\n  rotation: not documented\n  expiry: tied to the plan's validity period; renewal and upgrade are done from the dashboard\n  revocation: not documented\n  free_tier: >-\n    A free plan exists (2 req/s, 10,000 requests/day). The provider-published SKILL.md additionally\n    advertises a \"7-day free trial with full access\".\ngaps:\n  - No documented key-rotation or revocation procedure.\n  - No scope or permission model — a key is all-or-nothing within its plan entitlements.\n  - >-\n    The WebSocket surface accepts the key as a URL query parameter, which is weaker than a header and is not\n    flagged as a risk in the provider's documentation.\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n    - {url: 'https://infoway.readme.io/reference/api-key-application.md', http_status: 200}\n    - {url: 'https://infoway.readme.io/reference/ws-subscription.md', http_status: 200}\n    - {url: 'https://docs.infoway.io/sdk-and-tools/mcp-server.md', http_status:\
  \ 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoway-real-time-market-data-api/refs/heads/main/authentication/infoway-real-time-market-data-api-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- stock-api
- forex-api
- crypto-api
- commodities-api
- futures-api
- market-data
- real-time-data
- websocket
- financial-data
- fintech
- historical-data
---
