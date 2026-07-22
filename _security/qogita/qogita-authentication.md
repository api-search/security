---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Qogita Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Qogita secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Qogita
provider_slug: qogita
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization-code flow with PKCE (S256) protecting the Qogita hosted MCP resource, advertised via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata.
  flows:
  - authorizationUrl: https://api.qogita.com/staff/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://api.qogita.com/staff/oauth/register
    scopes:
      staff:mcp: Access to the Qogita Staff MCP server
    tokenUrl: https://api.qogita.com/staff/oauth/token
  issuer: https://api.qogita.com
  name: OAuth2
  sources:
  - well-known/qogita-oauth-authorization-server.json
  type: oauth2
slug: qogita-authentication
source_filename: qogita-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://api.qogita.com/.well-known/oauth-authorization-server +\n  https://api.qogita.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE (S256) protecting the Qogita\n    hosted MCP resource, advertised via RFC 8414 authorization-server metadata\n    and RFC 9728 protected-resource metadata.\n  issuer: https://api.qogita.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.qogita.com/staff/oauth/authorize\n    tokenUrl: https://api.qogita.com/staff/oauth/token\n    registrationUrl: https://api.qogita.com/staff/oauth/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    scopes:\n      staff:mcp:\
  \ Access to the Qogita Staff MCP server\n  sources:\n  - well-known/qogita-oauth-authorization-server.json\nnotes: >-\n  Auth profile derived from the published OAuth/OIDC discovery documents rather\n  than an OpenAPI spec (Qogita's REST API reference is a hosted Notion portal\n  with no downloadable OpenAPI). The buyer-facing REST API on api.qogita.com is\n  documented at developers.qogita.com; its auth scheme is not machine-readable\n  here and is therefore not asserted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qogita/refs/heads/main/authentication/qogita-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ecommerce
- Wholesale
- Marketplace
- Health and Beauty
- B2B
- Retail
- Distribution
---
