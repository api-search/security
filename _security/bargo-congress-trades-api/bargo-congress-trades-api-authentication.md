---
api_key_in:
- header
- query
api_specs:
- filename: bargo-congress-trades-api-members-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Members API
  slug: bargo-congress-trades-api-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-members-api-openapi.yml
- filename: bargo-congress-trades-api-statistics-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Statistics API
  slug: bargo-congress-trades-api-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-statistics-api-openapi.yml
- filename: bargo-congress-trades-api-trades-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Trades API
  slug: bargo-congress-trades-api-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-trades-api-openapi.yml
auth_types:
- apiKey
- http
description: 'Authentication for the Bargo Congress Trades API is OPTIONAL, which is the single most important fact about it: the OpenAPI top-level security array leads with an empty requirement, so anonymous callers are served at a lower quota rather than rejected. A free key — no card, self-serve — raises the quota and is the only way to call the Congress MCP endpoint''s tools. Three interchangeable credential presentations are declared; Bargo''s own agent skill ranks them.'
kind: authentication
layout: security
method: searched
name: Bargo Congress Trades Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bargo Congress Trades API secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bargo Congress Trades API
provider_slug: bargo-congress-trades-api
scheme_count: 3
schemes:
- description: Optional free Bargo API key.
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  preferred: true
  sources:
  - openapi/bargo-congress-trades-api-congress-trades-openapi.yml
  type: apiKey
- bearerFormat: Bargo API key
  description: Optional free Bargo API key as a Bearer token.
  name: BearerAuth
  preferred: false
  scheme: bearer
  sources:
  - openapi/bargo-congress-trades-api-congress-trades-openapi.yml
  type: http
- caution: A credential in a query string is logged by proxies and browser history. Bargo scopes this deliberately — its documentation says to use ?token= only for connector UIs (Claude/ChatGPT app connectors) that cannot set a header, and its own agent skill instructs agents to prefer X-Api-Key.
  description: Optional free Bargo API key for clients that cannot set headers.
  in: query
  name: QueryToken
  parameter: token
  preferred: false
  sources:
  - openapi/bargo-congress-trades-api-congress-trades-openapi.yml
  type: apiKey
slug: bargo-congress-trades-api-authentication
source_filename: bargo-congress-trades-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/bargo-congress-trades-api-congress-trades-openapi.yml\ndocs:\n  - https://www.bargo.ai/free-apis/congress\n  - https://www.bargo.ai/free-apis/dash\ndescription: >-\n  Authentication for the Bargo Congress Trades API is OPTIONAL, which is the\n  single most important fact about it: the OpenAPI top-level security array\n  leads with an empty requirement, so anonymous callers are served at a lower\n  quota rather than rejected. A free key — no card, self-serve — raises the\n  quota and is the only way to call the Congress MCP endpoint's tools. Three\n  interchangeable credential presentations are declared; Bargo's own agent skill\n  ranks them.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  required: false\n  anonymous_access: true\n  preferred_scheme: ApiKeyHeader\nschemes:\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    description: Optional\
  \ free Bargo API key.\n    preferred: true\n    sources:\n      - openapi/bargo-congress-trades-api-congress-trades-openapi.yml\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: Bargo API key\n    description: Optional free Bargo API key as a Bearer token.\n    preferred: false\n    sources:\n      - openapi/bargo-congress-trades-api-congress-trades-openapi.yml\n  - name: QueryToken\n    type: apiKey\n    in: query\n    parameter: token\n    description: Optional free Bargo API key for clients that cannot set headers.\n    preferred: false\n    caution: >-\n      A credential in a query string is logged by proxies and browser history.\n      Bargo scopes this deliberately — its documentation says to use ?token=\n      only for connector UIs (Claude/ChatGPT app connectors) that cannot set a\n      header, and its own agent skill instructs agents to prefer X-Api-Key.\n    sources:\n      - openapi/bargo-congress-trades-api-congress-trades-openapi.yml\ncredentials:\n\
  \  - id: free-api-key\n    prefix: fak_\n    issued_by: https://www.bargo.ai/free-apis/dash\n    cost: free\n    card_required: false\n    rotatable: true\n    authorizes:\n      - The Congress Trades REST API at https://www.bargo.ai/free-apis/congress/v1\n      - The focused Congress MCP endpoint at https://www.bargo.ai/free-apis/congress/mcp\n    does_not_authorize:\n      - Bargo's full market-intelligence MCP server at https://www.bargo.ai/mcp\n  - id: bargo-mcp-token\n    prefix: swmcp_\n    issued_by: 'https://www.bargo.ai (authorized account, then GET /api/mcp-token)'\n    scope: out-of-scope-for-this-repo\n    authorizes:\n      - Bargo's full MCP server at https://www.bargo.ai/mcp\n    note: >-\n      Recorded only to make the boundary explicit. Bargo states the separation\n      in three places — llms.txt, the MCP server card, and its published agent\n      skill — precisely because the two look interchangeable and are not.\nper_operation:\n  - operation: getCongressApiHealth\n\
  \    security: []\n    note: >-\n      The only operation that declares an EMPTY security array, meaning no\n      credential is accepted or required at all. Every other operation declares\n      401 InvalidKey and honours an optional key.\n  - operations:\n      - listCongressTrades\n      - listCongressTradesByTicker\n      - listCongressMembers\n      - getCongressMember\n      - getCongressTradeStats\n    security: inherited\n    note: >-\n      Inherit the top-level requirement [{}, ApiKeyHeader, BearerAuth,\n      QueryToken] — anonymous OR any one of the three key presentations.\nerror_behaviour:\n  '401': >-\n    Returned only when a key is supplied and is invalid or revoked. An absent key\n    is never a 401 — it is a lower quota.\n  '429': >-\n    The practical consequence of staying anonymous. See\n    rate-limits/bargo-congress-trades-api-rate-limits.yml\nhandling_guidance:\n  source: https://github.com/bargo-ai/bargo-free-api-packages/blob/main/skills/bargo-congress-api/SKILL.md\n\
  \  rules:\n    - Prefer X-Api-Key; Bearer is also supported; use the token query parameter only where headers are impossible.\n    - Never print, commit, log or return an API key.\n    - Never substitute a fak_ key for a swmcp_ credential or imply the free key unlocks Bargo's main MCP service.\n    - Pass keys through the environment or a secret manager, never in source.\ngaps:\n  - No OAuth 2.0 or OpenID Connect; /.well-known/oauth-authorization-server and /.well-known/openid-configuration both returned 404.\n  - No scopes, roles or permission model — a key is all-or-nothing over a read-only surface.\n  - No documented key rotation policy, expiry or revocation notification beyond the self-serve dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/authentication/bargo-congress-trades-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- congress
- finance
- stocks
- government
- stock-act
- mcp
- congressional-trading
- financial-disclosure
- market-data
- public-data
- free-api
- open-data
---
