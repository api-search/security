---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Seedlegals Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: SeedLegals secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: SeedLegals
provider_slug: seedlegals
scheme_count: 2
schemes:
- dynamic_client_registration: https://api.seedlegals.com/mcp/oauth2/register
  flows:
  - authorizationUrl: https://api.seedlegals.com/mcp/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://api.seedlegals.com/mcp/oauth2/token
    scopes:
    - openid
    - email
    - read
    - write
    tokenUrl: https://api.seedlegals.com/mcp/oauth2/token
  name: SeedLegals MCP OAuth2
  source: https://api.seedlegals.com/.well-known/oauth-authorization-server
  type: oauth2
- authorizationUrl: https://auth.seedlegals.com/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  dpop_supported: true
  end_session_endpoint: https://auth.seedlegals.com/oauth2/logout
  grant_types_supported:
  - authorization_code
  - password
  - implicit
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - client_credentials
  issuer: https://auth.seedlegals.com/6586e0bc-1d4b-ee88-2f82-7cbaa0189308
  name: SeedLegals Identity (FusionAuth OIDC)
  openIdConnectUrl: https://auth.seedlegals.com/.well-known/openid-configuration
  scopes:
  - openid
  - offline_access
  - email
  - phone
  - profile
  source: https://auth.seedlegals.com/.well-known/openid-configuration
  tokenUrl: https://auth.seedlegals.com/oauth2/token
  type: openIdConnect
  userinfoUrl: https://auth.seedlegals.com/oauth2/userinfo
slug: seedlegals-authentication
source_filename: seedlegals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://auth.seedlegals.com/.well-known/openid-configuration and\n  https://api.seedlegals.com/.well-known/oauth-authorization-server\ndocs: https://api.seedlegals.com/mcp\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken]\n  identity_provider: FusionAuth\n  notes: >-\n    SeedLegals has no publicly documented REST API; authentication is only\n    observable through published OAuth/OIDC discovery documents. The user-facing\n    application authenticates against a FusionAuth OpenID Connect provider at\n    auth.seedlegals.com. The agent-facing MCP server at api.seedlegals.com/mcp\n    exposes its own OAuth 2.0 authorization server (PKCE + dynamic client\n    registration).\nschemes:\n- name: SeedLegals MCP OAuth2\n  type: oauth2\n  source: https://api.seedlegals.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.seedlegals.com/mcp/oauth2/authorize\n\
  \    tokenUrl: https://api.seedlegals.com/mcp/oauth2/token\n    refreshUrl: https://api.seedlegals.com/mcp/oauth2/token\n    pkce: S256\n    scopes: [openid, email, read, write]\n  dynamic_client_registration: https://api.seedlegals.com/mcp/oauth2/register\n- name: SeedLegals Identity (FusionAuth OIDC)\n  type: openIdConnect\n  source: https://auth.seedlegals.com/.well-known/openid-configuration\n  issuer: https://auth.seedlegals.com/6586e0bc-1d4b-ee88-2f82-7cbaa0189308\n  openIdConnectUrl: https://auth.seedlegals.com/.well-known/openid-configuration\n  authorizationUrl: https://auth.seedlegals.com/oauth2/authorize\n  tokenUrl: https://auth.seedlegals.com/oauth2/token\n  userinfoUrl: https://auth.seedlegals.com/oauth2/userinfo\n  end_session_endpoint: https://auth.seedlegals.com/oauth2/logout\n  grant_types_supported:\n  - authorization_code\n  - password\n  - implicit\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - client_credentials\n  code_challenge_methods_supported:\
  \ [S256]\n  dpop_supported: true\n  scopes: [openid, offline_access, email, phone, profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seedlegals/refs/heads/main/authentication/seedlegals-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Business Applications
- Legal Tech
- Startups
- Fundraising
- Cap Table
- Equity
- Compliance
- MCP
- OpenID Connect
---
