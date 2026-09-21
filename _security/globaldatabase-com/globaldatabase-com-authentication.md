---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: globaldatabase-com-mcp-playground-openapi.yml
  format: yaml
  label: Global Database MCP Server
  slug: global-database-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-mcp-playground-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Globaldatabase Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Global Database secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Global Database
provider_slug: globaldatabase-com
scheme_count: 2
schemes:
- applies_to:
  - https://api.globaldatabase.com/v2/
  - https://api.globaldatabase.com/v2/ai/query (Regis AI query)
  challenge_observed: 'WWW-Authenticate: Token'
  error_shape: '{"detail": "Authentication credentials were not provided."} (401); docs name the invalid-token case TokenVerificationError -> {"detail": "Invalid token"}.'
  example_from_docs: 'Authorization: Token 00000000-0000-0000-0000-000000000000'
  in: header
  key_shape: UUID-looking token in the docs example (36 chars); the credential is issued per account.
  name: TokenAuth
  obtain: GlobalDatabase Profile on the platform (https://platform.globaldatabase.com) or via the account manager; free trial keys via https://platform.globaldatabase.com/public/signup/free_tier_ai.
  parameter_name: Authorization
  sources:
  - https://api.globaldatabase.com/docs/v2/#authentication
  - live 401 probe 2026-09-19
  type: apiKey
  value_format: Token <api-key>
- applies_to:
  - https://mcp.globaldatabase.com/mcp
  description: OAuth 2.1 authorization-code flow with PKCE (S256) and RFC 7591 dynamic client registration, fronting the MCP endpoint. Metadata is published per RFC 8414 and RFC 9728 on the MCP host.
  flows:
  - authorization_endpoint: https://mcp.globaldatabase.com/authorize
    authorization_server: https://mcp.globaldatabase.com/
    bearer_methods:
    - header
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registration_endpoint: https://mcp.globaldatabase.com/register
    resource: https://mcp.globaldatabase.com/mcp
    scopes: []
    scopes_note: 'scopes_supported is an empty array; clients must request no scope (README: a non-empty scope fails the token request in Copilot Studio).'
    token_endpoint: https://mcp.globaldatabase.com/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: McpOAuth
  sources:
  - well-known/globaldatabase-com-mcp-oauth-authorization-server.json
  - well-known/globaldatabase-com-mcp-oauth-protected-resource.json
  - https://github.com/global-database/mcp-server#authentication
  type: oauth2
slug: globaldatabase-com-authentication
source_filename: globaldatabase-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.globaldatabase.com/docs/v2/#authentication + https://mcp.globaldatabase.com/ + https://mcp.globaldatabase.com/.well-known/oauth-authorization-server + https://github.com/global-database/mcp-server#authentication\ndocs: https://api.globaldatabase.com/docs/v2/#authentication\nprobed: >-\n  2026-09-19 unauthenticated POST https://api.globaldatabase.com/v2/overview, POST /v2/ai/query\n  and GET /v2/metrics all returned HTTP 401 application/json {\"detail\":\"Authentication\n  credentials were not provided.\"} with `WWW-Authenticate: Token` — the Django REST Framework\n  TokenAuthentication challenge, matching the documented `Authorization: Token <key>` scheme.\n  POST https://mcp.globaldatabase.com/mcp returned 401 with `WWW-Authenticate: Bearer\n  error=\"invalid_token\" ... resource_metadata=\"https://mcp.globaldatabase.com/.well-known/oauth-protected-resource/mcp\"`.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in:\
  \ [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two surfaces, two schemes. The v2 REST API (api.globaldatabase.com) uses a static API key\n    sent as `Authorization: Token <key>` (not Bearer). The hosted MCP server uses OAuth 2.1\n    with PKCE and dynamic client registration; the user's REST API key is entered once in the\n    browser login page and bound into the access-token claims server-side, so it never travels\n    as a tool argument.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  value_format: 'Token <api-key>'\n  example_from_docs: 'Authorization: Token 00000000-0000-0000-0000-000000000000'\n  key_shape: 'UUID-looking token in the docs example (36 chars); the credential is issued per account.'\n  obtain: 'GlobalDatabase Profile on the platform (https://platform.globaldatabase.com) or via the account manager; free trial keys via https://platform.globaldatabase.com/public/signup/free_tier_ai.'\n  applies_to: [https://api.globaldatabase.com/v2/,\
  \ 'https://api.globaldatabase.com/v2/ai/query (Regis AI query)']\n  challenge_observed: 'WWW-Authenticate: Token'\n  error_shape: '{\"detail\": \"Authentication credentials were not provided.\"} (401); docs name the invalid-token case TokenVerificationError -> {\"detail\": \"Invalid token\"}.'\n  sources: [https://api.globaldatabase.com/docs/v2/#authentication, live 401 probe 2026-09-19]\n- name: McpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE (S256) and RFC 7591 dynamic client registration,\n    fronting the MCP endpoint. Metadata is published per RFC 8414 and RFC 9728 on the MCP host.\n  flows:\n  - flow: authorizationCode\n    authorization_server: https://mcp.globaldatabase.com/\n    authorization_endpoint: https://mcp.globaldatabase.com/authorize\n    token_endpoint: https://mcp.globaldatabase.com/token\n    registration_endpoint: https://mcp.globaldatabase.com/register\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n\
  \    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    scopes: []\n    scopes_note: 'scopes_supported is an empty array; clients must request no scope (README: a non-empty scope fails the token request in Copilot Studio).'\n    bearer_methods: [header]\n    resource: https://mcp.globaldatabase.com/mcp\n  applies_to: [https://mcp.globaldatabase.com/mcp]\n  sources: [well-known/globaldatabase-com-mcp-oauth-authorization-server.json, well-known/globaldatabase-com-mcp-oauth-protected-resource.json, https://github.com/global-database/mcp-server#authentication]\nsecurity_headers_observed:\n  api_host: [x-frame-options DENY, x-content-type-options nosniff, referrer-policy same-origin, cross-origin-opener-policy same-origin, 'strict-transport-security max-age=15724800; includeSubDomains']\n  mcp_host: [x-frame-options DENY, x-content-type-options nosniff, referrer-policy strict-origin-when-cross-origin, 'content-security-policy default-src ''self'' ...', 'strict-transport-security\
  \ max-age=15724800; includeSubDomains']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/authentication/globaldatabase-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Company Data
- KYB
- Compliance
- Business Verification
- Beneficial Ownership
- Financial
- Credit Risk
- Data Enrichment
- Prospecting
- Webhook
- MCP
- AI Agents
- United Kingdom
---
