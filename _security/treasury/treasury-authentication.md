---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Treasury Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Treasury secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Treasury
provider_slug: treasury
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://treasury.app/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://treasury.app/oauth/register
    scopes:
    - description: Connect to the Treasury Model Context Protocol (MCP) server.
      scope: mcp:connect
    tokenUrl: https://treasury.app/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  name: OAuth2
  sources:
  - well-known/treasury-oauth-authorization-server.json
  type: oauth2
slug: treasury-authentication
source_filename: treasury-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://treasury.app/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://treasury.app/oauth/authorize\n    tokenUrl: https://treasury.app/oauth/token\n    registrationUrl: https://treasury.app/oauth/register   # RFC 7591 dynamic client registration\n    pkce: S256\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    scopes:\n    - scope: mcp:connect\n      description: Connect to the Treasury Model Context Protocol (MCP) server.\n  sources: [well-known/treasury-oauth-authorization-server.json]\nnotes: >-\n  Auth profile derived from Treasury's published RFC 8414 OAuth Authorization\n  Server Metadata. This OAuth server guards the hosted MCP server at\n  https://treasury.app/mcp.\
  \ No traditional API-key or OpenAPI security scheme is\n  published (the consumer app has no public REST developer platform).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury/refs/heads/main/authentication/treasury-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Investing
- Personal Finance
- Fintech
- Brokerage
- Financial Education
- MCP
- Agent
---
