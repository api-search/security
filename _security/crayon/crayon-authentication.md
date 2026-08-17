---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Crayon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Crayon secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Crayon
provider_slug: crayon
scheme_count: 2
schemes:
- applies_to: https://mcp.crayon.co/mcp/
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://app.crayon.co/oauth/authorize/
    flow: authorizationCode
    issuer: https://app.crayon.co
    refresh_supported: true
    registrationUrl: https://app.crayon.co/oauth/register/
    revocationUrl: https://app.crayon.co/oauth/revoke_token/
    scopes:
      mcp:read: Read access to the Crayon competitive-intelligence MCP server
    tokenUrl: https://app.crayon.co/oauth/token/
  name: CrayonOAuth2
  sources:
  - well-known/crayon-oauth-authorization-server.json
  - well-known/crayon-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
- applies_to: https://mcp.crayon.co/mcp/
  name: BearerToken
  note: 'The protected-resource metadata declares bearer_methods_supported ["header"], and an unauthenticated POST returns WWW-Authenticate: Bearer error="invalid_token". The access token is carried in the Authorization header.'
  scheme: bearer
  sources:
  - well-known/crayon-oauth-protected-resource.json
  type: http
slug: crayon-authentication
source_filename: crayon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.crayon.co/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Crayon publishes no developer portal, API reference or auth guide. This profile is read entirely\n  from the machine-readable OAuth metadata the MCP host and app host serve anonymously (RFC 8414 +\n  RFC 9728) and from the 401 challenge the MCP endpoint returns. The earlier version of this file\n  was derived from a spec belonging to Crayon Group ASA (crayon.com) and has been quarantined —\n  see _wrong-company/README.md.\n\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  bearer: true\n  dynamic_client_registration: true\n  pkce_required_methods:\n  - S256\n\nschemes:\n- name: CrayonOAuth2\n  type: oauth2\n  applies_to: https://mcp.crayon.co/mcp/\n  flows:\n  - flow: authorizationCode\n    issuer: https://app.crayon.co\n    authorizationUrl: https://app.crayon.co/oauth/authorize/\n    tokenUrl: https://app.crayon.co/oauth/token/\n\
  \    revocationUrl: https://app.crayon.co/oauth/revoke_token/\n    registrationUrl: https://app.crayon.co/oauth/register/\n    refresh_supported: true\n    scopes:\n      mcp:read: Read access to the Crayon competitive-intelligence MCP server\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - none\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/crayon-oauth-authorization-server.json\n  - well-known/crayon-oauth-protected-resource.json\n- name: BearerToken\n  type: http\n  scheme: bearer\n  applies_to: https://mcp.crayon.co/mcp/\n  note: >-\n    The protected-resource metadata declares bearer_methods_supported [\"header\"], and an\n    unauthenticated POST returns WWW-Authenticate: Bearer error=\"invalid_token\". The access token\n    is carried in the Authorization header.\n  sources:\n  - well-known/crayon-oauth-protected-resource.json\n\nnot_documented:\n- >-\n  The Content API and Answers API that Crayon markets\
  \ have no published authentication model —\n  no key format, no header name, no token endpoint appears on any public page.\n\nx-evidence:\n- fetched: '2026-08-14'\n  url: https://mcp.crayon.co/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-14'\n  url: https://mcp.crayon.co/.well-known/oauth-protected-resource/mcp/\n  http_status: 200\n- fetched: '2026-08-14'\n  url: https://app.crayon.co/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-14'\n  url: https://mcp.crayon.co/mcp/\n  http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/authentication/crayon-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- Product Marketing
- AI
- MCP
---
