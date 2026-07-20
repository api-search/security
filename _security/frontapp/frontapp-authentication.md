---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Frontapp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: FrontApp secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: FrontApp
provider_slug: frontapp
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'API tokens (JWT bearer tokens) are created per company from Settings and passed in the Authorization header as `Authorization: Bearer <token>`. Recommended for single-company integrations and server-to-server access.'
  docs: https://dev.frontapp.com/docs/create-and-revoke-api-tokens
  name: apiToken
  scheme: bearer
  type: http
- description: OAuth 2.0 authorization code flow for building apps that access many Front companies. Access tokens expire after 60 minutes; refresh tokens are valid for 6 months (a new refresh token is issued in the final 24 hours before expiry). Scopes are selected at authorization time.
  docs: https://dev.frontapp.com/docs/oauth
  flows:
  - access_token_ttl_seconds: 3600
    authorizationUrl: https://app.frontapp.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.frontapp.com/oauth/token
    refresh_token_ttl: 6 months
    tokenUrl: https://app.frontapp.com/oauth/token
  name: oauth2
  type: oauth2
- description: OAuth 2.1 authorization server backing the Front MCP server; supports authorization_code, refresh_token, and client_credentials grants with PKCE (S256). Advertised via RFC 8414 metadata.
  flows:
  - authorizationUrl: https://app.frontapp.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://app.frontapp.com/oauth/revoke
    tokenUrl: https://app.frontapp.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://app.frontapp.com/oauth/token
  name: oauth2-mcp
  scopes:
  - feature:mcp
  source: well-known/frontapp-oauth-authorization-server.json
  type: oauth2
slug: frontapp-authentication
source_filename: frontapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.frontapp.com/docs/authentication\ndocs: https://dev.frontapp.com/docs/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  api_key_in: []\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    API tokens (JWT bearer tokens) are created per company from Settings and\n    passed in the Authorization header as `Authorization: Bearer <token>`.\n    Recommended for single-company integrations and server-to-server access.\n  docs: https://dev.frontapp.com/docs/create-and-revoke-api-tokens\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization code flow for building apps that access many Front\n    companies. Access tokens expire after 60 minutes; refresh tokens are valid\n    for 6 months (a new refresh token is issued in the final 24 hours before\n    expiry). Scopes\
  \ are selected at authorization time.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.frontapp.com/oauth/authorize\n    tokenUrl: https://app.frontapp.com/oauth/token\n    refreshUrl: https://app.frontapp.com/oauth/token\n    access_token_ttl_seconds: 3600\n    refresh_token_ttl: 6 months\n  docs: https://dev.frontapp.com/docs/oauth\n- name: oauth2-mcp\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization server backing the Front MCP server; supports\n    authorization_code, refresh_token, and client_credentials grants with PKCE\n    (S256). Advertised via RFC 8414 metadata.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.frontapp.com/oauth/authorize\n    tokenUrl: https://app.frontapp.com/oauth/token\n    revocationUrl: https://app.frontapp.com/oauth/revoke\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://app.frontapp.com/oauth/token\n  scopes: [feature:mcp]\n  source: well-known/frontapp-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontapp/refs/heads/main/authentication/frontapp-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Communication
- Customer Service
- Shared Inbox
- Email
- Messaging
- Collaboration
- Help Desk
---
