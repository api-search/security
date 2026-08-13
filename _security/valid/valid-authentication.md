---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Valid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valid declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Valid
provider_slug: valid
scheme_count: 3
schemes:
- authorization_url: https://mcp.valid.co/oauth/authorize
  bearer_methods_supported:
  - header
  dynamic_client_registration:
    endpoint: https://mcp.valid.co/oauth/register
    note: GET returns 405 Method Not Allowed; registration is POST-only, as specified.
    spec: RFC 7591
    supported: true
  flow: authorizationCode
  name: oauth2_authorization_code
  pkce:
    code_challenge_methods_supported:
    - S256
    - plain
    note: The server advertises `plain` alongside `S256`. RFC 7636 §4.2 and the OAuth 2.1 draft both require S256 where the client can support it; offering `plain` at all is a downgrade an attacker can request. This is the single weakest point in an otherwise strong auth posture.
    required: unknown
  refresh_supported: true
  registration_url: https://mcp.valid.co/oauth/register
  scopes:
    email: Account email address
    openid: OpenID Connect subject identifier
    profile: Basic profile claims
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  token_url: https://mcp.valid.co/oauth/token
  type: oauth2
- applies_to: Every path on mcp.valid.co and v1.valid-gke-data-api.com EXCEPT /health and the three OAuth/OIDC metadata documents.
  in: header
  name: outer_api_key
  name_note: The header name is not published. An unauthenticated request to any gated path returns HTTP 407 {"error":"API key missing"}, which names the credential class but not the header. HTTP 407 is Proxy Authentication Required and the response carries no Proxy-Authenticate header, so this gate is non-conformant with RFC 9110 §15.5.8.
  type: apiKey
- applies_to: https://mcp.valid.co/api/mcp/
  evidence: 'HTTP 401 with `www-authenticate: Bearer` and body {"detail":"Not authenticated"} on an anonymous JSON-RPC tools/list POST.'
  name: mcp_bearer
  scheme: bearer
  type: http
slug: valid-authentication
source_filename: valid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://mcp.valid.co/.well-known/oauth-authorization-server and\n  https://mcp.valid.co/.well-known/oauth-protected-resource (both HTTP 200,\n  fetched 2026-08-12), plus observed WWW-Authenticate and error responses.\ndocs: null\ndocs_note: >-\n  Valid publishes no developer authentication page. This profile is derived\n  entirely from the machine-readable metadata the server itself serves and from\n  live unauthenticated responses.\napi: Valid Chat With Your Ads MCP Server\nschemes:\n- name: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://mcp.valid.co/oauth/authorize\n  token_url: https://mcp.valid.co/oauth/token\n  registration_url: https://mcp.valid.co/oauth/register\n  refresh_supported: true\n  scopes:\n    openid: OpenID Connect subject identifier\n    email: Account email address\n    profile: Basic profile claims\n  pkce:\n    required: unknown\n    code_challenge_methods_supported:\
  \ [S256, plain]\n    note: >-\n      The server advertises `plain` alongside `S256`. RFC 7636 §4.2 and the\n      OAuth 2.1 draft both require S256 where the client can support it; offering\n      `plain` at all is a downgrade an attacker can request. This is the single\n      weakest point in an otherwise strong auth posture.\n  dynamic_client_registration:\n    supported: true\n    endpoint: https://mcp.valid.co/oauth/register\n    spec: RFC 7591\n    note: GET returns 405 Method Not Allowed; registration is POST-only, as specified.\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  bearer_methods_supported: [header]\n- name: outer_api_key\n  type: apiKey\n  in: header\n  name_note: >-\n    The header name is not published. An unauthenticated request to any gated path\n    returns HTTP 407 {\"error\":\"API key missing\"}, which names the credential class\n    but not the header. HTTP 407 is Proxy Authentication Required and the response\n\
  \    carries no Proxy-Authenticate header, so this gate is non-conformant with\n    RFC 9110 §15.5.8.\n  applies_to: >-\n    Every path on mcp.valid.co and v1.valid-gke-data-api.com EXCEPT /health and the\n    three OAuth/OIDC metadata documents.\n- name: mcp_bearer\n  type: http\n  scheme: bearer\n  applies_to: https://mcp.valid.co/api/mcp/\n  evidence: >-\n    HTTP 401 with `www-authenticate: Bearer` and body {\"detail\":\"Not authenticated\"}\n    on an anonymous JSON-RPC tools/list POST.\nopenid_connect:\n  discovery_url: https://mcp.valid.co/.well-known/openid-configuration\n  status: 200\n  conformant: false\n  note: >-\n    The document served at the OIDC discovery path is byte-identical to the RFC 8414\n    OAuth document. It omits every OIDC-required field — no `jwks_uri`, no\n    `userinfo_endpoint`, no `subject_types_supported`, no\n    `id_token_signing_alg_values_supported` — so despite advertising the `openid`\n    scope this is an OAuth 2.0 authorization server metadata\
  \ document served at an\n    OIDC path, not an OpenID Provider configuration.\nposture:\n  summary: >-\n    Strong for an unadvertised agent endpoint: OAuth 2.1-shaped authorization code\n    flow with refresh tokens, PKCE, RFC 7591 dynamic client registration, RFC 8414\n    authorization server metadata and RFC 9728 protected resource metadata — the\n    full MCP authorization discovery chain, correctly wired. Weakened by `plain`\n    PKCE remaining on offer, a non-conformant 407 outer gate, and the absence of any\n    published authentication documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valid/refs/heads/main/authentication/valid-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative
- Media Buying
- Influencers
- MCP
- Agents
- Performance Marketing
---
