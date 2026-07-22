---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lightyear Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lightyear secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lightyear
provider_slug: lightyear
scheme_count: 1
schemes:
- dynamic_client_registration:
    registration_endpoint: https://api.lightyear.com/oauth2/internal-mcp/register
    standard: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://api.lightyear.com/oauth2/internal-mcp/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    refresh: true
    scopes:
    - mcp
    tokenUrl: https://api.lightyear.com/oauth2/internal-mcp/token
  issuer: https://api.lightyear.com
  jwks_uri: https://api.lightyear.com/.well-known/jwks.json
  name: internal-mcp
  sources:
  - well-known/lightyear-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: lightyear-authentication
source_filename: lightyear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.lightyear.com/.well-known/oauth-authorization-server\nnotes: >-\n  Lightyear publishes no public developer API and no developer authentication documentation. The\n  only machine-readable auth surface found is the RFC 8414 OAuth 2.0 authorization server metadata\n  served from api.lightyear.com, which describes an OAuth 2.0 authorization-code + PKCE flow scoped\n  to an internal MCP integration. It is captured here as observed fact, not as a documented public\n  auth contract for third-party developers.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: internal-mcp\n  type: oauth2\n  issuer: https://api.lightyear.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.lightyear.com/oauth2/internal-mcp/authorize\n    tokenUrl: https://api.lightyear.com/oauth2/internal-mcp/token\n    refresh: true\n    pkce_methods:\n    - S256\n    scopes:\n\
  \    - mcp\n  dynamic_client_registration:\n    supported: true\n    standard: RFC 7591\n    registration_endpoint: https://api.lightyear.com/oauth2/internal-mcp/register\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  jwks_uri: https://api.lightyear.com/.well-known/jwks.json\n  sources:\n  - well-known/lightyear-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightyear/refs/heads/main/authentication/lightyear-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Financial Services
- Investing
- Brokerage
- Stocks
- ETFs
- Fintech
- Wealth Management
- Europe
---
