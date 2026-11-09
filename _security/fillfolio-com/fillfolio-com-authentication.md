---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Fillfolio public API
  slug: fillfolio-public-api
  spec_type: OpenAPI
  url: https://fillfolio.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fillfolio Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fillfolio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fillfolio
provider_slug: fillfolio-com
scheme_count: 1
schemes:
- authorization_url: https://fillfolio.com/oauth/authorize
  bearer_methods:
  - header
  code_challenge_methods:
  - S256
  flow: authorization_code
  name: oauth2_pkce
  notes: OAuth 2.0 authorization-code with PKCE S256 for MCP access. Public PKCE clients (no client secret). Pre-registered client IDs only; general Dynamic Client Registration is disabled. The advertised /oauth/register endpoint serves only the dedicated Docker MCP Gateway public client. Tokens are bound to the MCP resource https://fillfolio.com/api/mcp. Access tokens expire after 10 minutes; refresh tokens rotate, expire after 30 days of non-use and cannot extend a connection beyond 90 days. Reusing a spent code or refresh token revokes its token family. No OIDC ID tokens are issued. Query-string tokens are rejected.
  pkce_required: true
  revocation_url: https://fillfolio.com/oauth/revoke
  scopes:
  - mcp:read
  token_url: https://fillfolio.com/oauth/token
  type: oauth2
slug: fillfolio-com-authentication
source_filename: fillfolio-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fillfolio.com/auth.md\ndocs: https://fillfolio.com/auth.md\nschemes:\n- name: oauth2_pkce\n  type: oauth2\n  flow: authorization_code\n  authorization_url: https://fillfolio.com/oauth/authorize\n  token_url: https://fillfolio.com/oauth/token\n  revocation_url: https://fillfolio.com/oauth/revoke\n  pkce_required: true\n  code_challenge_methods:\n  - S256\n  scopes:\n  - mcp:read\n  bearer_methods:\n  - header\n  notes: >-\n    OAuth 2.0 authorization-code with PKCE S256 for MCP access. Public PKCE clients\n    (no client secret). Pre-registered client IDs only; general Dynamic Client\n    Registration is disabled. The advertised /oauth/register endpoint serves only\n    the dedicated Docker MCP Gateway public client. Tokens are bound to the MCP\n    resource https://fillfolio.com/api/mcp. Access tokens expire after 10 minutes;\n    refresh tokens rotate, expire after 30 days of non-use and cannot extend a\n    connection\
  \ beyond 90 days. Reusing a spent code or refresh token revokes its\n    token family. No OIDC ID tokens are issued. Query-string tokens are rejected.\nresource:\n  url: https://fillfolio.com/api/mcp\n  audience: https://fillfolio.com/api/mcp\n  metadata:\n    protected_resource: https://fillfolio.com/.well-known/oauth-protected-resource/api/mcp\n    authorization_server: https://fillfolio.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/fillfolio-com/authentication/fillfolio-com-authentication.yml
summary_line: 1 scheme
tags:
- Portfolio Tracking
- Net Worth
- Personal Finance
- Investment Tracking
- Bank Aggregation
- Crypto Wallet Tracking
- MCP
- Google Sheets Add-on
---
