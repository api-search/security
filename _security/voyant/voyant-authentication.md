---
api_key_in: []
api_specs:
- filename: voyant-openapi-original.json
  format: json
  label: VoyantIO API
  slug: voyantio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/openapi/voyant-openapi-original.json
- filename: voyant-gypsum-openapi.json
  format: json
  label: Gypsum Context API
  slug: gypsum-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/openapi/voyant-gypsum-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Voyant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voyant.io secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voyant.io
provider_slug: voyant
scheme_count: 2
schemes:
- applied_to_operations: 672
  bearer_format: null
  name: HTTPBearer
  note: A single `http bearer` scheme with no `bearerFormat`, no scopes and no OAuth flows, carrying two structurally different credentials (a long-lived opaque API key and a short-lived Clerk session token) through the same header. A client cannot tell from the contract which one an operation expects, and the contract offers no way to express least privilege.
  scheme: bearer
  sources:
  - openapi/voyant-openapi-original.json
  surface: VoyantIO API (783 operations)
  token_forms:
  - evidence: GET /mcp/health publishes auth_methods ["api_key (vio_*)","clerk_token"]; the agent-samples .env template uses API_KEY=vio_xxxxxxxxxxxxxxxxxx.
    form: api-key
    issued_where: Settings > API Keys (per the agent-samples README)
    prefix: vio_
  - evidence: 'info.description: "Most endpoints require a Bearer token from Clerk authentication." The marketing SPA bundles the Clerk browser SDK.'
    form: clerk-session-token
  type: http
  unsecured_operations: 111
- evidence: 'info.description: "Most endpoints require `user_id` query parameter (Clerk organization ID). Demo access is available for testing." The contract declares NO components.securitySchemes and NO security requirement on any operation — the scheme exists only in prose.'
  in: query
  name: user_id query parameter
  note: 'A tenant identifier in the query string is the weakest pattern on this provider''s surface: it lands in server logs, proxy logs, Referer headers and browser history. It is also not an authenticator — an organization ID is an identifier, and nothing in the published contract shows a secret being presented alongside it. Cannot be verified live: gypsum.voyant.io is NXDOMAIN.'
  parameter: user_id
  security_schemes_declared: 0
  sources:
  - openapi/voyant-gypsum-openapi.json
  surface: Gypsum Context API (26 operations)
  type: apiKey
slug: voyant-authentication
source_filename: voyant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/voyant-openapi-original.json (components.securitySchemes + per-operation security),\n  openapi/voyant-gypsum-openapi.json (info.description auth section),\n  https://voice-forge-production.up.railway.app/mcp/health (published auth_methods),\n  https://github.com/andrew-brown-noosphere/agent-samples (.env template naming the key prefix)\ndocs: null\ndocs_note: >-\n  Voyant publishes no authentication page. There is no developer portal beyond the FastAPI\n  /docs and /redoc renderings of the spec, and neither carries an auth guide. Everything below\n  was assembled from the contracts themselves plus live endpoint payloads.\nsummary:\n  types:\n    - http\n    - apiKey\n  oauth2: false\n  openIdConnect: false\n  mutualTLS: false\n  identity_provider: Clerk\n  note: >-\n    Three different authentication models across three surfaces, none of them documented in one\n    place: bearer token on the main REST API, `vio_*`\
  \ API key or Clerk token on the MCP server,\n    and a `user_id` QUERY PARAMETER on the Gypsum contract.\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    bearer_format: null\n    surface: VoyantIO API (783 operations)\n    applied_to_operations: 672\n    unsecured_operations: 111\n    sources:\n      - openapi/voyant-openapi-original.json\n    token_forms:\n      - form: api-key\n        prefix: vio_\n        evidence: >-\n          GET /mcp/health publishes auth_methods [\"api_key (vio_*)\",\"clerk_token\"]; the\n          agent-samples .env template uses API_KEY=vio_xxxxxxxxxxxxxxxxxx.\n        issued_where: 'Settings > API Keys (per the agent-samples README)'\n      - form: clerk-session-token\n        evidence: >-\n          info.description: \"Most endpoints require a Bearer token from Clerk authentication.\"\n          The marketing SPA bundles the Clerk browser SDK.\n    note: >-\n      A single `http bearer` scheme with no `bearerFormat`, no scopes and no\
  \ OAuth flows, carrying\n      two structurally different credentials (a long-lived opaque API key and a short-lived Clerk\n      session token) through the same header. A client cannot tell from the contract which one an\n      operation expects, and the contract offers no way to express least privilege.\n  - name: user_id query parameter\n    type: apiKey\n    in: query\n    parameter: user_id\n    surface: Gypsum Context API (26 operations)\n    security_schemes_declared: 0\n    sources:\n      - openapi/voyant-gypsum-openapi.json\n    evidence: >-\n      info.description: \"Most endpoints require `user_id` query parameter (Clerk organization ID).\n      Demo access is available for testing.\" The contract declares NO components.securitySchemes\n      and NO security requirement on any operation — the scheme exists only in prose.\n    note: >-\n      A tenant identifier in the query string is the weakest pattern on this provider's surface:\n      it lands in server logs, proxy logs,\
  \ Referer headers and browser history. It is also not an\n      authenticator — an organization ID is an identifier, and nothing in the published contract\n      shows a secret being presented alongside it. Cannot be verified live: gypsum.voyant.io is\n      NXDOMAIN.\nunauthenticated_surface:\n  operation_count: 111\n  note: >-\n    111 of 783 operations on the main API declare no security. The genuinely-public subset is the\n    telemetry ingestion path (POST /api/telemetry/track, /api/telemetry/end-session,\n    /api/deo/ingest, /api/deo/v1/telemetry/events, /api/deo/v1/traces, /api/deo/mcp-telemetry),\n    which is intentional and rate-limited per IP at 100 req/min, plus /health, /mcp/* and the\n    /api/well-known/* generators. The remainder has not been audited operation by operation and\n    is the highest-value security review this provider could run on itself.\n  probed:\n    - url: https://voice-forge-production.up.railway.app/api/context-streams/streaming/architecture\n    \
  \  status: 200\n      note: Anonymous read of the streaming topology — public by design.\n    - url: https://voice-forge-production.up.railway.app/api/context-streams/streaming/available-streams\n      status: 401\n      note: '{\"detail\":\"Authentication required\"} — gating works where it is applied.'\n    - url: https://voice-forge-production.up.railway.app/mcp/tools\n      status: 200\n      note: Full tool list with inputSchemas, anonymous. Discovery open, invocation closed.\nscopes:\n  supported: false\n  note: >-\n    No OAuth flows, no scopes, no permissions model anywhere in either contract. A token is\n    all-or-nothing across 783 operations, including the four operations classified\n    safety-critical in agentic-access/voyant-agentic-access.yml. Nothing was written to scopes/.\noauth_discovery:\n  authorization_server_metadata: false\n  protected_resource_metadata: false\n  note: >-\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource are\
  \ soft\n    404s (HTML shell) on www.voyant.io and 405 on the API host. An MCP client that expects the\n    2026 OAuth handshake finds nothing to negotiate against — the server takes a static key\n    instead.\ngaps:\n  - No published authentication documentation of any kind.\n  - No bearerFormat, so key format is discoverable only from a health payload and a sample repo.\n  - No scopes; no least-privilege story for a 783-operation surface.\n  - Three auth models across three surfaces, each documented in a different artifact's prose.\n  - Gypsum's auth model puts a tenant identifier in the query string.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/authentication/voyant-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Artificial Intelligence
- Context Management
- Brand Governance
- Product Marketing
- gtm-operations
- Marketing Automation
- Content Generation
- Competitive Intelligence
- Semantic Search
- RAG
- MCP
- agent-native
- Signals
- Telemetry
---
