---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Openart Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Openart secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Openart
provider_slug: openart
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://openart.ai/suite/api/auth/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    registrationUrl: https://openart.ai/suite/api/auth/oauth/register
    revocationUrl: https://openart.ai/suite/api/auth/oauth/revoke
    scopes:
      full_access: Full access to the authenticated OpenArt account
    tokenEndpointAuthMethods:
    - none
    tokenUrl: https://openart.ai/suite/api/auth/oauth/token
  name: OAuth2
  sources:
  - well-known/openart-oauth-authorization-server.json
  type: oauth2
slug: openart-authentication
source_filename: openart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openart.ai/.well-known/oauth-authorization-server\ndocs: https://openart.ai/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\n  public_clients: true\n  scopes: [full_access]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://openart.ai/suite/api/auth/oauth/authorize\n    tokenUrl: https://openart.ai/suite/api/auth/oauth/token\n    registrationUrl: https://openart.ai/suite/api/auth/oauth/register\n    revocationUrl: https://openart.ai/suite/api/auth/oauth/revoke\n    codeChallengeMethods: [S256]\n    grantTypes: [authorization_code, refresh_token]\n    tokenEndpointAuthMethods: [none]\n    scopes:\n      full_access: Full access to the authenticated OpenArt account\n  sources: [well-known/openart-oauth-authorization-server.json]\nnotes: >-\n  OpenArt's authenticated surface is its remote\
  \ MCP server\n  (https://mcp.openart.ai/mcp). Authentication is OAuth 2.0 Authorization Code\n  with PKCE and RFC 7591 Dynamic Client Registration; clients are public\n  (no client secret). OpenID Connect discovery is also published. No public REST\n  API key program is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openart/refs/heads/main/authentication/openart-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Creative Tools
- MCP
- Model Context Protocol
---
