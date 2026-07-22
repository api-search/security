---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Noredink Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NoRedInk secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NoRedInk
provider_slug: noredink
scheme_count: 2
schemes:
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - roles
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.noredink.com
  name: OpenIDConnect
  openIdConnectUrl: https://www.noredink.com/.well-known/openid-configuration
  sources:
  - well-known/noredink-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- endpoints:
    authorization: https://www.noredink.com/oauth/authorize
    introspection: https://www.noredink.com/oauth/introspect
    jwks: https://www.noredink.com/oauth/discovery/keys
    revocation: https://www.noredink.com/oauth/revoke
    token: https://www.noredink.com/oauth/token
    userinfo: https://www.noredink.com/oauth/userinfo
  flows:
  - authorizationUrl: https://www.noredink.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://www.noredink.com/oauth/token
    scopes:
      openid: OpenID Connect authentication (sign-in / identity)
    tokenUrl: https://www.noredink.com/oauth/token
  name: OAuth2
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  sources:
  - well-known/noredink-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: noredink-authentication
source_filename: noredink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  well-known/noredink-openid-configuration.json,\n  well-known/noredink-oauth-authorization-server.json\ndocs: https://www.noredink.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  grant_types:\n  - authorization_code\n  - refresh_token\n  issuer: https://www.noredink.com\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.noredink.com/.well-known/openid-configuration\n  issuer: https://www.noredink.com\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - roles\n  sources:\n  - well-known/noredink-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.noredink.com/oauth/authorize\n    tokenUrl: https://www.noredink.com/oauth/token\n\
  \    refreshUrl: https://www.noredink.com/oauth/token\n    scopes:\n      openid: OpenID Connect authentication (sign-in / identity)\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\n  - fragment\n  - form_post\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  endpoints:\n    authorization: https://www.noredink.com/oauth/authorize\n    token: https://www.noredink.com/oauth/token\n    revocation: https://www.noredink.com/oauth/revoke\n    introspection: https://www.noredink.com/oauth/introspect\n    userinfo: https://www.noredink.com/oauth/userinfo\n    jwks: https://www.noredink.com/oauth/discovery/keys\n  sources:\n  - well-known/noredink-oauth-authorization-server.json\nnotes: >-\n  Derived from NoRedInk's published OpenID Connect discovery and RFC 8414\n  authorization-server metadata. NoRedInk operates a standards-based OAuth 2.0\n  authorization-code + refresh-token flow with OpenID Connect on top (RS256 id\n\
  \  tokens, userinfo, JWKS, token introspection and revocation). Only the `openid`\n  scope is advertised in discovery. This is an SSO / partner-integration surface\n  rather than an open public data API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noredink/refs/heads/main/authentication/noredink-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Education
- EdTech
- English Language Arts
- Grammar
- Writing
- Literacy
- K-12
- OAuth
- OpenID Connect
- Single Sign-On
- Rostering
- Identity
---
