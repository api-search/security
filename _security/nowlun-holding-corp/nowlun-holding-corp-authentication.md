---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nowlun Holding Corp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nowlun Holding Corp. secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nowlun Holding Corp.
provider_slug: nowlun-holding-corp
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://nowlun.com/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    issuer: https://nowlun.com
    jwksUri: https://nowlun.com/oauth/discovery/keys
    revocationUrl: https://nowlun.com/oauth/revoke
    scopes:
    - excel
    - mcp
    - mind
    tokenUrl: https://nowlun.com/oauth/token
  name: OAuth2
  sources:
  - well-known/nowlun-holding-corp-oauth-authorization-server.json
  type: oauth2
slug: nowlun-holding-corp-authentication
source_filename: nowlun-holding-corp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nowlun.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    issuer: https://nowlun.com\n    authorizationUrl: https://nowlun.com/oauth/authorize\n    tokenUrl: https://nowlun.com/oauth/token\n    revocationUrl: https://nowlun.com/oauth/revoke\n    jwksUri: https://nowlun.com/oauth/discovery/keys\n    grantTypes: [authorization_code, refresh_token]\n    codeChallengeMethods: [S256]\n    scopes: [excel, mcp, mind]\n  sources: [well-known/nowlun-holding-corp-oauth-authorization-server.json]\nnotes: >-\n  Auth model derived from Nowlun's published RFC 8414 authorization-server metadata.\n  Authorization Code + PKCE (S256) with refresh tokens. No dynamic client registration\n  endpoint discovered.\
  \ The MCP server at https://nowlun.com/mcp is gated on the \"mcp\" scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowlun-holding-corp/refs/heads/main/authentication/nowlun-holding-corp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Logistics
- Freight Forwarding
- Shipping
- Supply Chain
- Sea Freight
- Customs
- MENA
- MCP
---
