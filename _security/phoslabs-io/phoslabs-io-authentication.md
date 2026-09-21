---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: phoslabs-io-openapi.yml
  format: yaml
  label: Behavioral Science API
  slug: behavioral-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-openapi.yml
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Phoslabs Io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Phos Labs secures its APIs with http, oauth2, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Phos Labs
provider_slug: phoslabs-io
scheme_count: 3
schemes:
- description: API key from /api/trial or purchased at /credits
  header: 'Authorization: Bearer <api_key>'
  name: BearerAuth
  observed:
  - 'POST /api/v1/diagnose without the header -> 401 {"error": "Missing Authorization header. Use: Authorization: Bearer <api_key>"}'
  - 'POST /api/v1/diagnose with an invalid key -> 401 {"error": "Invalid or inactive API key"}; no WWW-Authenticate header'
  scheme: bearer
  sources:
  - openapi/phoslabs-io-openapi.yml
  type: http
- dynamic_client_registration: https://mcp.phoslabs.io/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.phoslabs.io/authorize
      refreshUrl: https://mcp.phoslabs.io/token
      scopes:
        claudeai: null
      tokenUrl: https://mcp.phoslabs.io/token
  name: mcp-oauth
  observed:
  - 'POST /mcp (initialize) -> 401 WWW-Authenticate: Bearer error="invalid_token", error_description="Authentication required", resource_metadata="https://mcp.phoslabs.io/.well-known/oauth-protected-resource/mcp"'
  pkce: S256
  protected_resource: https://mcp.phoslabs.io/mcp
  revocation: https://mcp.phoslabs.io/revoke
  sources:
  - well-known/phoslabs-io-oauth-authorization-server.json
  - well-known/phoslabs-io-oauth-protected-resource-mcp.json
  type: oauth2
- applies_to:
  - https://mcp.phoslabs.io/sse
  - https://mcp.phoslabs.io/messages
  header: 'Authorization: Bearer <key>'
  in: header
  name: mcp-sse-api-key
  observed:
  - 'GET /sse -> 401 {"error":"unauthorized","message":"API key required. Pass Authorization: Bearer <key> header."}'
  sources:
  - live probe 2026-09-19
  type: apiKey
slug: phoslabs-io-authentication
source_filename: phoslabs-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/phoslabs-io-openapi.yml\ndocs:\n- https://github.com/phoslabs/behavioral-science-api#access-methods\n- https://phoslabs.io/api/v1/tools\n- https://mcp.phoslabs.io/.well-known/oauth-authorization-server\n- https://mcp.phoslabs.io/.well-known/oauth-protected-resource/mcp\nsummary:\n  types: [http, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  surfaces:\n  - {surface: 'REST https://phoslabs.io/api/v1/*', auth: 'Bearer API key (http bearer)', anonymous_operations: [listTools]}\n  - {surface: 'MCP https://mcp.phoslabs.io/mcp (Streamable HTTP)', auth: 'OAuth 2.1 authorization code + PKCE, dynamic client registration'}\n  - {surface: 'MCP https://mcp.phoslabs.io/sse and /messages (legacy SSE)', auth: 'API key as Bearer token'}\n  - {surface: 'x402 https://phoslabs.io/x402/* (stated)', auth: 'USDC on Base L2 per call — every path returned 403 on 2026-09-19; unverified'}\nkey_issuance:\n  self_serve:\
  \ true\n  method: 'POST https://phoslabs.io/api/trial with {\"email\": \"...\", \"name\": \"...\"} (per GET /api/v1/tools get_key); GET on the path is 405'\n  free_credits: '100 for new accounts (README) / 20 on MCP connect (credits page)'\n  purchase: https://phoslabs.io/credits\n  note: Not exercised; no key was provisioned by this probe.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key from /api/trial or purchased at /credits\n  header: 'Authorization: Bearer <api_key>'\n  sources: [openapi/phoslabs-io-openapi.yml]\n  observed:\n  - 'POST /api/v1/diagnose without the header -> 401 {\"error\": \"Missing Authorization header. Use: Authorization: Bearer <api_key>\"}'\n  - 'POST /api/v1/diagnose with an invalid key -> 401 {\"error\": \"Invalid or inactive API key\"}; no WWW-Authenticate header'\n- name: mcp-oauth\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.phoslabs.io/authorize\n      tokenUrl: https://mcp.phoslabs.io/token\n\
  \      refreshUrl: https://mcp.phoslabs.io/token\n      scopes: {claudeai: null}\n  pkce: S256\n  dynamic_client_registration: https://mcp.phoslabs.io/register\n  revocation: https://mcp.phoslabs.io/revoke\n  protected_resource: https://mcp.phoslabs.io/mcp\n  sources: [well-known/phoslabs-io-oauth-authorization-server.json, well-known/phoslabs-io-oauth-protected-resource-mcp.json]\n  observed:\n  - 'POST /mcp (initialize) -> 401 WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"Authentication required\", resource_metadata=\"https://mcp.phoslabs.io/.well-known/oauth-protected-resource/mcp\"'\n- name: mcp-sse-api-key\n  type: apiKey\n  in: header\n  header: 'Authorization: Bearer <key>'\n  applies_to: ['https://mcp.phoslabs.io/sse', 'https://mcp.phoslabs.io/messages']\n  sources: [live probe 2026-09-19]\n  observed:\n  - 'GET /sse -> 401 {\"error\":\"unauthorized\",\"message\":\"API key required. Pass Authorization: Bearer <key> header.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/authentication/phoslabs-io-authentication.yml
summary_line: http/oauth2/apiKey · 3 schemes
tags:
- Company
- Behavioral Science
- Conversion Optimization
- E-Commerce
- Pricing
- Copywriting
- AI Agents
- MCP
- A2A
- Decision Intelligence
- Agentic Commerce
---
