---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Realscout Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RealScout secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RealScout
provider_slug: realscout
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.realscout.com/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    grant_types_supported:
    - authorization_code
    - refresh_token
    issuer: https://www.realscout.com
    jwksUri: https://www.realscout.com/.well-known/mcp/jwks.json
    registrationUrl: https://www.realscout.com/oauth/register
    response_types_supported:
    - code
    revocationUrl: https://www.realscout.com/oauth/revoke
    scopes:
      mcp: Access to the RealScout admin MCP server (api://realscout-admin-mcp)
    sources:
    - well-known/realscout-oauth-authorization-server.json
    tokenUrl: https://www.realscout.com/oauth/token
    token_endpoint_auth_methods_supported:
    - none
  name: OAuth2
  type: oauth2
slug: realscout-authentication
source_filename: realscout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.realscout.com/.well-known/oauth-authorization-server\ndocs: https://www.realscout.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        issuer: https://www.realscout.com\n        authorizationUrl: https://www.realscout.com/oauth/authorize\n        tokenUrl: https://www.realscout.com/oauth/token\n        registrationUrl: https://www.realscout.com/oauth/register   # RFC 7591\n        revocationUrl: https://www.realscout.com/oauth/revoke        # RFC 7009\n        jwksUri: https://www.realscout.com/.well-known/mcp/jwks.json\n        scopes:\n          mcp: Access to the RealScout admin MCP server (api://realscout-admin-mcp)\n        code_challenge_methods_supported: [S256]\n        token_endpoint_auth_methods_supported:\
  \ [none]   # public clients (PKCE)\n        response_types_supported: [code]\n        grant_types_supported: [authorization_code, refresh_token]\n        sources: [well-known/realscout-oauth-authorization-server.json]\nnotes: >-\n  Auth model derived from RealScout's live RFC 8414 authorization-server metadata,\n  which backs the hosted MCP server. This OAuth 2.1 surface is the only publicly\n  documented authentication. RealScout also advertises \"direct API access\" and\n  \"SAML / SSO\" on Enterprise plans (learn.realscout.com/pricing), but no public\n  OpenAPI or developer auth docs are published for that API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realscout/refs/heads/main/authentication/realscout-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Real Estate
- PropTech
- Lead Nurture
- Home Search
- MLS
- MCP
- Artificial Intelligence
---
