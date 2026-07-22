---
api_key_in: []
api_specs:
- filename: zippykid-pressable-openapi-original.json
  format: json
  label: Pressable API
  slug: pressable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/openapi/zippykid-pressable-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zippykid Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ZippyKid secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ZippyKid
provider_slug: zippykid
scheme_count: 2
schemes:
- applied_as: Authorization Bearer <access_token>
  description: API v1 authenticates with OAuth 2.0 client-credentials. A client_id and client_secret are generated in the My Pressable Control Panel and exchanged for a Bearer access token valid for one hour. Request a new token before the current one expires; tokens can be revoked.
  flows:
  - flow: clientCredentials
    grant_type: client_credentials
    revocationUrl: https://my.pressable.com/auth/revoke
    tokenUrl: https://my.pressable.com/auth/token
  name: OAuth2ClientCredentials
  sources:
  - https://my.pressable.com/documentation/api/v1/authentication.md
  type: oauth2
- description: 'Pressable''s remote MCP server uses a distinct OAuth authorization-code flow with PKCE (S256) and dynamic client registration, advertised via RFC 8414 metadata at /.well-known/oauth-authorization-server. Scope: mcp. An Access Token from the control panel may be used as an alternative credential.'
  flows:
  - authorizationUrl: https://my.pressable.com/auth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://my.pressable.com/auth/register
    tokenUrl: https://my.pressable.com/auth/token
  name: MCPOAuth
  sources:
  - https://my.pressable.com/.well-known/oauth-authorization-server
  type: oauth2
slug: zippykid-authentication
source_filename: zippykid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://my.pressable.com/documentation/api/v1/authentication.md\ndocs: https://my.pressable.com/documentation/api/v1\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  token_lifetime_seconds: 3600\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  description: >-\n    API v1 authenticates with OAuth 2.0 client-credentials. A client_id and\n    client_secret are generated in the My Pressable Control Panel and exchanged\n    for a Bearer access token valid for one hour. Request a new token before the\n    current one expires; tokens can be revoked.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://my.pressable.com/auth/token\n    revocationUrl: https://my.pressable.com/auth/revoke\n    grant_type: client_credentials\n  applied_as: Authorization Bearer <access_token>\n  sources: [https://my.pressable.com/documentation/api/v1/authentication.md]\n- name: MCPOAuth\n \
  \ type: oauth2\n  description: >-\n    Pressable's remote MCP server uses a distinct OAuth authorization-code flow\n    with PKCE (S256) and dynamic client registration, advertised via RFC 8414\n    metadata at /.well-known/oauth-authorization-server. Scope: mcp. An Access\n    Token from the control panel may be used as an alternative credential.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.pressable.com/auth/authorize\n    tokenUrl: https://my.pressable.com/auth/token\n    registrationUrl: https://my.pressable.com/auth/register\n    pkce: S256\n  sources: [https://my.pressable.com/.well-known/oauth-authorization-server]\nnotes: >-\n  The published OpenAPI does not declare securitySchemes (components empty), so\n  this profile is sourced from the human docs and the well-known metadata rather\n  than derived. See scopes/zippykid-scopes.yml for the permission model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/authentication/zippykid-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- WordPress
- Managed Hosting
- WordPress Hosting
- Web Hosting
- WP Cloud
- MCP
- DevOps
---
