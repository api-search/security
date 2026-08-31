---
api_key_in:
- header
api_specs:
- filename: improvado-ask-api-openapi.yml
  format: yaml
  label: Improvado Ask API
  slug: improvado-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/improvado/refs/heads/main/openapi/improvado-ask-api-openapi.yml
auth_types:
- http
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Improvado Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Improvado secures its APIs with http, oauth2, and none across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Improvado
provider_slug: improvado
scheme_count: 5
schemes:
- description: RFC 7617 HTTP Basic. Credentials (username:password, base64) are provisioned by Improvado for Embedded API access; the customer changes the password on first use. Required for workspace management and for calling POST /api/v3/token to mint a workspace-scoped Bearer token. Invalid credentials return 401 Unauthorized.
  name: basicAuth
  scheme: basic
  type: http
  used_for:
  - workspace management
  - token acquisition
- bearerFormat: opaque
  description: 'Workspace-scoped access token obtained from POST /api/v3/token. Sent as Authorization: Bearer <token>. Required for workspace-specific resources (connections, accounts, extracts, destinations, data tables, loads, recipes, roles, webhooks). Token TTL is 30 minutes, renewed on each authorized use; an invalid or expired token returns 401 Unauthorized.'
  name: bearerToken
  scheme: bearer
  type: http
  used_for:
  - workspace-scoped resources
- description: Cookie-based session used by embedded-UI (iframe) flows, combined with an X-IM-WORKSPACE-ID request header to scope the session to a workspace.
  in: cookie
  name: cookieSession
  parameterName: dts_session_id
  type: apiKey
  used_for:
  - embedded iframe UI
- cross_link: scopes/improvado-scopes.yml
  description: OAuth 2.0 authorization server on the customer's own Improvado tenant domain, gating the 84-tool customer MCP endpoint. Authorization code grant with PKCE (plain and S256), refresh tokens, dynamic client registration (RFC 7591) and client_id metadata documents. Bearer token in the Authorization header. Improvado's positioning is "your existing Improvado credentials, no new tokens to manage" — the agent authorizes as the human, it does not get its own API key.
  discovery:
    authorization_server_metadata: https://report.improvado.io/.well-known/oauth-authorization-server
    protected_resource_metadata: https://report.improvado.io/.well-known/oauth-protected-resource/experimental/agent/api/mcp-customer/v1/invoke/
    rfcs:
    - RFC 8414
    - RFC 9728
    - RFC 7591
    - RFC 7636
  flows:
  - authorizationUrl: https://report.improvado.io/api/dts/v2/oauth/o/authorize/
    flow: authorizationCode
    introspectionUrl: https://report.improvado.io/api/dts/v2/oauth/o/introspect/
    pkce:
    - plain
    - S256
    registrationUrl: https://report.improvado.io/api/dts/v2/oauth/o/register/
    revocationUrl: https://report.improvado.io/api/dts/v2/oauth/o/revoke_token/
    scopes:
    - mcp:customer
    tokenUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/
  host_note: The issuer is the tenant's own domain. On a whitelabel domain (e.g. acme.improvado.io), report.improvado.io will NOT authenticate the client — Improvado states this explicitly.
  method: probed
  name: improvadoOAuth
  session_ttl: 15 minutes (Redis-backed, workspace-scoped)
  source: https://report.improvado.io/.well-known/oauth-authorization-server
  surface: Improvado Customer MCP
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  used_for:
  - MCP tool calls
- description: 'POST https://agent.improvado.io/ask requires no authentication. The published OpenAPI declares no securitySchemes and its info.description states "This endpoint is open and does not require authentication." Improvado''s llms.txt adds the usage boundary: one public non-sensitive question, never send credentials or personal data, abusive bulk traffic may be rate limited.'
  method: searched
  name: none
  source: https://improvado.io/openapi.json
  surface: Improvado Public Agent Ask API
  type: none
  used_for:
  - public product and architecture Q&A
slug: improvado-authentication
source_filename: improvado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.improvado.io/auth\ndocs: https://developers.improvado.io/auth\nupdate_note: >-\n  UPDATED 2026-08-13. The 2026-07-19 profile covered only the Embedded API v3 and recorded\n  oauth2_flows: []. That is still correct for embedded.improvado.io, but Improvado runs THREE distinct\n  API surfaces with three different auth models, and the other two were missing. Added below: a full\n  OAuth 2.0 authorization-code + PKCE model on the tenant host (report.improvado.io) that gates the\n  customer MCP server — probed directly from its RFC 8414 and RFC 9728 metadata documents — and the\n  anonymous public Agent Ask endpoint.\nsummary:\n  types: [http, oauth2, none]\n  http_schemes: [basic, bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  surfaces: 3\n  notes: >-\n    Three surfaces. (1) Embedded API v3 (embedded.improvado.io) — two-stage: HTTP Basic (RFC 7617) for\n    workspace-management operations\
  \ and to obtain a workspace-scoped access token; the resulting Bearer\n    token for all workspace-scoped resources; plus a cookie/session variant (dts_session_id) with an\n    X-IM-WORKSPACE-ID header for embedded-UI sessions. (2) Customer MCP (report.improvado.io or a\n    whitelabel tenant domain) — OAuth 2.0 authorization code with PKCE, scope mcp:customer, dynamic\n    client registration, 15-minute workspace-scoped sessions. (3) Public Agent Ask API\n    (agent.improvado.io) — no authentication at all.\nsurfaces:\n- surface: Improvado Embedded API v3\n  host: https://embedded.improvado.io\n  schemes: [basicAuth, bearerToken, cookieSession]\n  docs: https://developers.improvado.io/auth\n- surface: Improvado Customer MCP\n  host: https://report.improvado.io (or a whitelabel tenant domain)\n  schemes: [improvadoOAuth]\n  docs: https://improvado.io/docs-section-topic/improvado-mcp\n  cross_link: scopes/improvado-scopes.yml\n- surface: Improvado Public Agent Ask API\n  host: https://agent.improvado.io\n\
  \  schemes: [none]\n  docs: https://improvado.io/llms.txt\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    RFC 7617 HTTP Basic. Credentials (username:password, base64) are provisioned by\n    Improvado for Embedded API access; the customer changes the password on first use.\n    Required for workspace management and for calling POST /api/v3/token to mint a\n    workspace-scoped Bearer token. Invalid credentials return 401 Unauthorized.\n  used_for: [workspace management, token acquisition]\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: >-\n    Workspace-scoped access token obtained from POST /api/v3/token. Sent as\n    Authorization: Bearer <token>. Required for workspace-specific resources\n    (connections, accounts, extracts, destinations, data tables, loads, recipes,\n    roles, webhooks). Token TTL is 30 minutes, renewed on each authorized use;\n    an invalid or expired token returns 401 Unauthorized.\n\
  \  used_for: [workspace-scoped resources]\n- name: cookieSession\n  type: apiKey\n  in: cookie\n  parameterName: dts_session_id\n  description: >-\n    Cookie-based session used by embedded-UI (iframe) flows, combined with an\n    X-IM-WORKSPACE-ID request header to scope the session to a workspace.\n  used_for: [embedded iframe UI]\n- name: improvadoOAuth\n  type: oauth2\n  surface: Improvado Customer MCP\n  method: probed\n  source: https://report.improvado.io/.well-known/oauth-authorization-server\n  description: >-\n    OAuth 2.0 authorization server on the customer's own Improvado tenant domain, gating the\n    84-tool customer MCP endpoint. Authorization code grant with PKCE (plain and S256), refresh\n    tokens, dynamic client registration (RFC 7591) and client_id metadata documents. Bearer token in\n    the Authorization header. Improvado's positioning is \"your existing Improvado credentials, no new\n    tokens to manage\" — the agent authorizes as the human, it does not get its\
  \ own API key.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://report.improvado.io/api/dts/v2/oauth/o/authorize/\n    tokenUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/\n    revocationUrl: https://report.improvado.io/api/dts/v2/oauth/o/revoke_token/\n    introspectionUrl: https://report.improvado.io/api/dts/v2/oauth/o/introspect/\n    registrationUrl: https://report.improvado.io/api/dts/v2/oauth/o/register/\n    pkce: [plain, S256]\n    scopes: [mcp:customer]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  session_ttl: 15 minutes (Redis-backed, workspace-scoped)\n  discovery:\n    authorization_server_metadata: https://report.improvado.io/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://report.improvado.io/.well-known/oauth-protected-resource/experimental/agent/api/mcp-customer/v1/invoke/\n    rfcs: [RFC 8414, RFC 9728, RFC 7591, RFC 7636]\n  used_for: [MCP tool calls]\n  cross_link: scopes/improvado-scopes.yml\n\
  \  host_note: >-\n    The issuer is the tenant's own domain. On a whitelabel domain (e.g. acme.improvado.io),\n    report.improvado.io will NOT authenticate the client — Improvado states this explicitly.\n- name: none\n  type: none\n  surface: Improvado Public Agent Ask API\n  method: searched\n  source: https://improvado.io/openapi.json\n  description: >-\n    POST https://agent.improvado.io/ask requires no authentication. The published OpenAPI declares no\n    securitySchemes and its info.description states \"This endpoint is open and does not require\n    authentication.\" Improvado's llms.txt adds the usage boundary: one public non-sensitive question,\n    never send credentials or personal data, abusive bulk traffic may be rate limited.\n  used_for: [public product and architecture Q&A]\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://report.improvado.io/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://report.improvado.io/experimental/agent/api/mcp-customer/v1/invoke/\n\
  \  http_status: 401\n  note: 'WWW-Authenticate: Bearer resource_metadata=\"...\", scope=\"mcp:customer\"'\n- fetched: '2026-08-13'\n  url: https://improvado.io/openapi.json\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://developers.improvado.io/auth.md\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improvado/refs/heads/main/authentication/improvado-authentication.yml
summary_line: http/oauth2/none · 5 schemes
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Analytics
- Data Pipeline
- ETL
- Advertising Data
- Business Intelligence
- Data Integration
- AI Agents
- MCP
- Agent Readiness
---
