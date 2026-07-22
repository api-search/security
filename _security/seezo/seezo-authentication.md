---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Seezo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Seezo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Seezo
provider_slug: seezo
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://app.seezo.io/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://app.seezo.io/oauth/revoke_token/
    tokenUrl: https://app.seezo.io/oauth/token/
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://app.seezo.io
  name: OAuth2
  registration_endpoint: https://app.seezo.io/oauth/register/
  response_types_supported:
  - code
  sources:
  - well-known/seezo-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: seezo-authentication
source_filename: seezo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.seezo.io/.well-known/oauth-authorization-server\nnotes: >-\n  Seezo publishes no OpenAPI, so this profile is derived from the provider's\n  live RFC 8414 OAuth 2.0 Authorization Server metadata document rather than\n  from a spec. The Seezo web app (app.seezo.io) authenticates end users; there\n  is no publicly documented developer/data API.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://app.seezo.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.seezo.io/oauth/authorize\n    tokenUrl: https://app.seezo.io/oauth/token/\n    revocationUrl: https://app.seezo.io/oauth/revoke_token/\n  registration_endpoint: https://app.seezo.io/oauth/register/\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n\
  \  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  sources:\n  - well-known/seezo-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seezo/refs/heads/main/authentication/seezo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai
- Security
- Application Security
- Threat Modeling
- Security Design Review
- Developer Tools
- DevSecOps
---
