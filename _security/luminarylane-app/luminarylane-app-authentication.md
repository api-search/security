---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Luminarylane App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luminary Lane secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Luminary Lane
provider_slug: luminarylane-app
scheme_count: 2
schemes:
- description: 'OAuth 2.1-style authorization-code flow advertised through RFC 8414 metadata; the MCP endpoint''s 401 carries WWW-Authenticate: Bearer error="invalid_token", resource_metadata="https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp", which is the MCP authorization specification''s discovery hand-off. An anonymous RFC 7591 POST to /register returned 201 with a client_id and client_secret (expiry ~30 days), so a client can self-register without a developer account. No scopes_supported is published anywhere.'
  dynamic_client_registration: https://mcp.luminarylane.app/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.luminarylane.app/authorize
      refreshUrl: https://mcp.luminarylane.app/token
      scopes: {}
      tokenUrl: https://mcp.luminarylane.app/token
  name: OAuth2
  pkce: S256 (required per code_challenge_methods_supported)
  revocation: https://mcp.luminarylane.app/revoke
  sources:
  - https://mcp.luminarylane.app/.well-known/oauth-authorization-server
  - https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
- description: 'Per-user API key generated at https://app.luminarylane.app/profile/api-keys (signed-in users; the path 307s to /login anonymously). Keys start with "ll_mcp_" and are shown once. The provider''s lane-plugin ships an .mcp.json that sends the key as an X-API-Key header on the Streamable HTTP connection, and its README bridges stdio-only clients with npx -y mcp-remote https://mcp.luminarylane.app/mcp --header X-API-Key:${LANE_API_KEY}. Observed: an invalid key returns 401 {"error":"Invalid API key"}.'
  in: header
  key_prefix: ll_mcp_
  name: ApiKeyHeader
  name_header: X-API-Key
  sources:
  - https://github.com/luminarylane/lane-plugin#setup
  - https://github.com/luminarylane/lane-plugin/blob/main/.mcp.json
  type: apiKey
slug: luminarylane-app-authentication
source_filename: luminarylane-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://github.com/luminarylane/lane-plugin#setup\ndocs: https://github.com/luminarylane/lane-plugin\ncorroborating_sources:\n  - https://mcp.luminarylane.app/.well-known/oauth-authorization-server\n  - https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\n  - https://app.luminarylane.app/api/health\nspec: null\nsummary:\n  types:\n    - oauth2\n    - apiKey\n  transport: HTTPS only; Authorization Bearer header (OAuth) or X-API-Key header (static key)\n  note: >-\n    Luminary Lane publishes no OpenAPI, so this profile was built from the live MCP endpoint's\n    challenge and discovery documents plus the provider's own plugin README — derive-authentication.py\n    correctly reports 0 auth profiles for this repo. The one public API surface, the remote MCP server\n    at https://mcp.luminarylane.app/mcp, accepts two credential shapes: an OAuth 2.1 bearer token\n    minted by the authorization server co-hosted\
  \ on mcp.luminarylane.app, or a static per-user API\n    key sent as X-API-Key. The product application itself (app.luminarylane.app) signs users in\n    through Auth0 — its /api/health check names an \"auth0\" dependency — but no Auth0 tenant metadata\n    is published and the app's API routes redirect anonymous callers to /login.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.luminarylane.app/authorize\n        tokenUrl: https://mcp.luminarylane.app/token\n        refreshUrl: https://mcp.luminarylane.app/token\n        scopes: {}\n    pkce: S256 (required per code_challenge_methods_supported)\n    dynamic_client_registration: https://mcp.luminarylane.app/register\n    revocation: https://mcp.luminarylane.app/revoke\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - none\n    description: >-\n      OAuth 2.1-style authorization-code flow advertised through RFC 8414 metadata; the MCP endpoint's\n\
  \      401 carries WWW-Authenticate: Bearer error=\"invalid_token\", resource_metadata=\"https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\",\n      which is the MCP authorization specification's discovery hand-off. An anonymous RFC 7591 POST to\n      /register returned 201 with a client_id and client_secret (expiry ~30 days), so a client can\n      self-register without a developer account. No scopes_supported is published anywhere.\n    sources:\n      - https://mcp.luminarylane.app/.well-known/oauth-authorization-server\n      - https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    name_header: X-API-Key\n    key_prefix: ll_mcp_\n    description: >-\n      Per-user API key generated at https://app.luminarylane.app/profile/api-keys (signed-in users;\n      the path 307s to /login anonymously). Keys start with \"ll_mcp_\" and are shown once. The\n      provider's lane-plugin ships an .mcp.json\
  \ that sends the key as an X-API-Key header on the\n      Streamable HTTP connection, and its README bridges stdio-only clients with\n      npx -y mcp-remote https://mcp.luminarylane.app/mcp --header X-API-Key:${LANE_API_KEY}.\n      Observed: an invalid key returns 401 {\"error\":\"Invalid API key\"}.\n    sources:\n      - https://github.com/luminarylane/lane-plugin#setup\n      - https://github.com/luminarylane/lane-plugin/blob/main/.mcp.json\ncredentials:\n  - id: oauth-access-token\n    header: 'Authorization: Bearer <access_token>'\n    prefix: null\n    use: MCP client sessions negotiated through the authorization-code + PKCE flow\n    issued_by: https://mcp.luminarylane.app/ (issuer)\n  - id: user-api-key\n    header: 'X-API-Key: ll_mcp_...'\n    prefix: ll_mcp_\n    use: MCP client sessions from Claude Desktop / Cowork and any client that can set a static header\n    issued_by: Luminary Lane app, Profile -> API Keys\n    note: Requires a paid Luminary Lane account with at least\
  \ one brand set up (plugin prerequisites).\nobserved_challenges:\n  - request: POST https://mcp.luminarylane.app/mcp (initialize, no credential)\n    status: 401\n    www_authenticate: 'Bearer error=\"invalid_token\", error_description=\"Missing Authorization header\", resource_metadata=\"https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\"'\n    body: '{\"error\":\"invalid_token\",\"error_description\":\"Missing Authorization header\"}'\n  - request: 'POST https://mcp.luminarylane.app/mcp (tools/list, X-API-Key: invalid)'\n    status: 401\n    body: '{\"error\":\"Invalid API key\"}'\n  - request: GET https://app.luminarylane.app/api\n    status: 307\n    location: /login?callbackUrl=%2Fapi\n    note: The product app's own API is session-gated behind Auth0 login; no public reference exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminarylane-app/refs/heads/main/authentication/luminarylane-app-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Marketing
- Marketing Automation
- AI Agents
- Agent-Native
- MCP
- A2A
- Brand Management
- Content Generation
- Campaign Management
- Social Media
- Software-as-a-Service
---
