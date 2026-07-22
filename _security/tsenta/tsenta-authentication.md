---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tsenta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tsenta secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tsenta
provider_slug: tsenta
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.autojobs.me/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://api.autojobs.me/oauth/register
    response_types:
    - code
    revocationUrl: https://api.autojobs.me/oauth/revoke
    tokenUrl: https://api.autojobs.me/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://api.autojobs.me
  name: OAuth2
  sources:
  - well-known/tsenta-oauth-authorization-server.json
  type: oauth2
slug: tsenta-authentication
source_filename: tsenta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.autojobs.me/.well-known/oauth-authorization-server\ndocs: https://tsenta.com/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  public_client: true            # token_endpoint_auth_methods_supported = [\"none\"]\n  dynamic_client_registration: true\nschemes:\n  - name: OAuth2\n    type: oauth2\n    issuer: https://api.autojobs.me\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.autojobs.me/oauth/authorize\n        tokenUrl: https://api.autojobs.me/oauth/token\n        registrationUrl: https://api.autojobs.me/oauth/register   # RFC 7591 dynamic client registration\n        revocationUrl: https://api.autojobs.me/oauth/revoke        # RFC 7009 token revocation\n        response_types: [code]\n        grant_types: [authorization_code, refresh_token]\n        code_challenge_methods: [S256]\n        token_endpoint_auth_methods: [none]\n    sources:\
  \ [well-known/tsenta-oauth-authorization-server.json]\nnotes: >-\n  Tsenta's API (api.autojobs.me) uses OAuth 2.0 / 2.1-style authorization-code\n  flow with PKCE (S256) for public clients and RFC 7591 dynamic client\n  registration — the modern pattern for authorizing AI agents / MCP clients.\n  No scopes are advertised in the authorization-server metadata. Sign-in is\n  federated via Google on the Tsenta approval screen; issued tokens are\n  short-lived and auto-refresh.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsenta/refs/heads/main/authentication/tsenta-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Jobs
- Recruiting
- Job Search
- AI Agents
- Automation
- Applicant Tracking
- Career
- MCP
- Y Combinator
---
