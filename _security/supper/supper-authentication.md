---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Supper Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Supper secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Supper
provider_slug: supper
scheme_count: 1
schemes:
- applies_to:
  - https://api.supper.co/mcp
  flows:
  - authorizationUrl: https://api.supper.co/mcp/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://api.supper.co/mcp/register
    scopes: {}
    tokenUrl: https://api.supper.co/mcp/token
    token_endpoint_auth_methods:
    - none
  issuer: https://api.supper.co
  name: OAuth2
  type: oauth2
slug: supper-authentication
source_filename: supper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.supper.co/.well-known/oauth-authorization-server\ndocs: https://www.supper.co/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  public_client: true          # token_endpoint_auth_methods_supported: none\n  pkce: S256\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://api.supper.co\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.supper.co/mcp/authorize\n    tokenUrl: https://api.supper.co/mcp/token\n    registrationUrl: https://api.supper.co/mcp/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    scopes: {}                 # scopes_supported not advertised in AS metadata\n  applies_to:\n  - https://api.supper.co/mcp\nnotes: >-\n  Authentication profile derived from Supper's published RFC 8414 OAuth 2.0\n  Authorization Server Metadata\
  \ and the /mcp connection docs. Supper's MCP\n  server is an OAuth 2.0 public client (PKCE S256) supporting Dynamic Client\n  Registration; end users authorize via one-click OAuth in Claude. No API-key\n  or basic-auth surface is documented publicly (developer docs are gated).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supper/refs/heads/main/authentication/supper-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Data
- Analytics
- Artificial Intelligence
- MCP
- Business Intelligence
- Semantic Layer
- Data Agent
---
