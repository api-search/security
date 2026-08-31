---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Articulate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
- deviceCode
overview: Articulate secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refresh_token, and deviceCode flow(s).
provider_name: Articulate
provider_slug: articulate
scheme_count: 2
schemes:
- issuer: https://id.articulate.com
  name: OpenIDConnect
  openIdConnectUrl: https://id.articulate.com/.well-known/openid-configuration
  sources:
  - well-known/articulate-openid-configuration.json
  type: openIdConnect
- endpoints:
    authorization: https://id.articulate.com/oauth2/v1/authorize
    jwks: https://id.articulate.com/oauth2/v1/keys
    registration: https://id.articulate.com/oauth2/v1/clients
    token: https://id.articulate.com/oauth2/v1/token
    userinfo: https://id.articulate.com/oauth2/v1/userinfo
  flows:
  - authorizationUrl: https://id.articulate.com/oauth2/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://id.articulate.com/oauth2/v1/token
  - authorizationUrl: https://id.articulate.com/oauth2/v1/authorize
    flow: implicit
  - flow: deviceCode
    tokenUrl: https://id.articulate.com/oauth2/v1/token
  issuer: https://id.articulate.com
  name: OAuth2
  sources:
  - well-known/articulate-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: oauth2
slug: articulate-authentication
source_filename: articulate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://id.articulate.com/.well-known/openid-configuration\ndocs: https://id.articulate.com/.well-known/openid-configuration\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refresh_token\n  - deviceCode\n  pkce: true\n  note: >-\n    Articulate does not publish a public developer REST API. Its programmatic\n    surface is the id.articulate.com identity provider (Okta-hosted), which\n    exposes standard OpenID Connect / OAuth 2.0 discovery used to authenticate\n    users into Articulate 360, Rise, Reach 360, and Review. No first-party\n    API-key or bearer-token developer credential is documented publicly.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://id.articulate.com/.well-known/openid-configuration\n  issuer: https://id.articulate.com\n  sources:\n  - well-known/articulate-openid-configuration.json\n- name: OAuth2\n  type:\
  \ oauth2\n  issuer: https://id.articulate.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.articulate.com/oauth2/v1/authorize\n    tokenUrl: https://id.articulate.com/oauth2/v1/token\n    pkce: S256\n  - flow: implicit\n    authorizationUrl: https://id.articulate.com/oauth2/v1/authorize\n  - flow: deviceCode\n    tokenUrl: https://id.articulate.com/oauth2/v1/token\n  endpoints:\n    authorization: https://id.articulate.com/oauth2/v1/authorize\n    token: https://id.articulate.com/oauth2/v1/token\n    userinfo: https://id.articulate.com/oauth2/v1/userinfo\n    jwks: https://id.articulate.com/oauth2/v1/keys\n    registration: https://id.articulate.com/oauth2/v1/clients\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  sources:\n  - well-known/articulate-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/articulate/refs/heads/main/authentication/articulate-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Edtech
- E-Learning
- Learning Management
- Training
- Course Authoring
- SSO
- OpenID Connect
---
