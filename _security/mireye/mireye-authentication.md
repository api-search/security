---
api_key_in: []
api_specs:
- filename: mireye-openapi-original.json
  format: json
  label: Mireye Earth API
  slug: mireye-earth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mireye Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mireye secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mireye
provider_slug: mireye
scheme_count: 3
schemes:
- applies_to:
  - POST /v1/ask
  - POST /v1/ask/stream
  - POST /v1/fetch
  - /v1/users/me/*
  bearer_format: JWT
  description: 'Dashboard-minted API token (JWT, 90-day default lifetime) sent as `Authorization: Bearer <token>` on all /v1/ask, /v1/fetch, and /v1/users/me/* requests. No API-key query params or custom headers.'
  name: bearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.1 + PKCE for the hosted MCP endpoint (/mcp). MCP clients discover the authorization server via /.well-known/oauth-authorization-server and complete a browser flow automatically. Tokens are scoped to MCP tool calls and are NOT accepted as general /v1/* API tokens.
  flows:
  - authorizationUrl: https://api.mireye.com/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.mireye.com/register
    revocationUrl: https://api.mireye.com/revoke
    scopes:
      mcp:tools: Call Mireye MCP tools (mireye_ask, mireye_fetch)
    tokenUrl: https://api.mireye.com/token
  name: mcpOAuth
  type: oauth2
- description: 'Device-authorization flow used by the local stdio adapter (`mireye-mcp login`): POST /v1/mcp/device/start -> browser approval -> POST /v1/mcp/device/poll, storing an API token in ~/.config/mireye-mcp/credentials.json bound to MIREYE_BASE_URL.'
  name: deviceFlow
  type: oauth2-device
slug: mireye-authentication
source_filename: mireye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mireye.ai/authentication\ndocs: https://docs.mireye.ai/authentication\nnote: >-\n  The published OpenAPI (openapi/mireye-openapi-original.json) declares no\n  components.securitySchemes, so this profile is captured from the docs auth page rather\n  than derived from the spec.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Dashboard-minted API token (JWT, 90-day default lifetime) sent as\n    `Authorization: Bearer <token>` on all /v1/ask, /v1/fetch, and /v1/users/me/* requests.\n    No API-key query params or custom headers.\n  applies_to: [POST /v1/ask, POST /v1/ask/stream, POST /v1/fetch, /v1/users/me/*]\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 + PKCE for the hosted MCP endpoint (/mcp). MCP clients discover the\n    authorization\
  \ server via /.well-known/oauth-authorization-server and complete a browser\n    flow automatically. Tokens are scoped to MCP tool calls and are NOT accepted as general\n    /v1/* API tokens.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mireye.com/authorize\n    tokenUrl: https://api.mireye.com/token\n    registrationUrl: https://api.mireye.com/register\n    revocationUrl: https://api.mireye.com/revoke\n    pkce: S256\n    scopes:\n      mcp:tools: Call Mireye MCP tools (mireye_ask, mireye_fetch)\n- name: deviceFlow\n  type: oauth2-device\n  description: >-\n    Device-authorization flow used by the local stdio adapter (`mireye-mcp login`):\n    POST /v1/mcp/device/start -> browser approval -> POST /v1/mcp/device/poll, storing an\n    API token in ~/.config/mireye-mcp/credentials.json bound to MIREYE_BASE_URL.\npublic_endpoints:\n- GET /healthz\n- GET /readyz\n- GET /v1/meta/fields\n- GET /v1/openapi.json\n- GET /v1/docs\nidentity_provider: Firebase (Google\
  \ or email/password with verified address)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/authentication/mireye-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- Model Context Protocol
- Government Data
- Risk
- Insurance
- Data
---
