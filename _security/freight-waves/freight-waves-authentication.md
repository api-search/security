---
api_key_in: []
api_specs:
- filename: freight-waves-sonar-openapi.yml
  format: yaml
  label: SONAR API
  slug: sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/openapi/freight-waves-sonar-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Freight Waves Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Freight Waves secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Freight Waves
provider_slug: freight-waves
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'SONAR REST API bearer token from POST /Credential/authenticate, sent as `Authorization: Bearer <token>`. Tokens are valid for one year; re-authenticating issues a new token without invalidating prior tokens.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freight-waves-sonar-openapi.yml
  - https://api.sonar.surf/Help/
  type: http
- description: OAuth 2.1 protection for the FreightWaves MCP server (scope mcp:read).
  flows:
  - authorizationUrl: https://api.freightwaves.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.freightwaves.com/oauth/register
    scopes:
      mcp:read: Read-only access to SONAR data via the MCP server.
    tokenUrl: https://api.freightwaves.com/oauth/token
  name: mcpOAuth
  sources:
  - well-known/freight-waves-oauth-authorization-server.json
  - well-known/freight-waves-oauth-protected-resource.json
  type: oauth2
slug: freight-waves-authentication
source_filename: freight-waves-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/freight-waves-sonar-openapi.yml\ndocs: https://api.sonar.surf/Help/\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  Two distinct auth surfaces. (1) The SONAR REST API uses an opaque/JWT bearer\n  token obtained from POST /Credential/authenticate (username + password), valid\n  one year, sent as `Authorization: Bearer <token>`. (2) The hosted MCP server at\n  api.freightwaves.com/mcp uses OAuth 2.1 (authorization_code + PKCE S256, dynamic\n  client registration, public client) with the mcp:read scope.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    SONAR REST API bearer token from POST /Credential/authenticate, sent as\n    `Authorization: Bearer <token>`. Tokens are valid for one year; re-authenticating\n    issues a new token without invalidating prior tokens.\n  sources:\n  - openapi/freight-waves-sonar-openapi.yml\n\
  \  - https://api.sonar.surf/Help/\n- name: mcpOAuth\n  type: oauth2\n  description: OAuth 2.1 protection for the FreightWaves MCP server (scope mcp:read).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freightwaves.com/oauth/authorize\n    tokenUrl: https://api.freightwaves.com/oauth/token\n    registrationUrl: https://api.freightwaves.com/oauth/register\n    pkce: S256\n    scopes:\n      mcp:read: Read-only access to SONAR data via the MCP server.\n  sources:\n  - well-known/freight-waves-oauth-authorization-server.json\n  - well-known/freight-waves-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/authentication/freight-waves-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Freight
- Logistics
- Supply Chain
- Transportation
- Trucking
- Market Data
- Analytics
- Freight Rates
- SONAR
---
