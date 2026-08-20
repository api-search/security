---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Place Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
- ciba
overview: PLACE secures its APIs with openIdConnect and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, deviceCode, and ciba flow(s).
provider_name: PLACE
provider_slug: place
scheme_count: 3
schemes:
- code_challenge_methods:
  - S256
  endpoints:
    authorization: https://sso.place.com/oauth2/v1/authorize
    device_authorization: https://sso.place.com/oauth2/v1/device/authorize
    end_session: https://sso.place.com/oauth2/v1/logout
    introspection: https://sso.place.com/oauth2/v1/introspect
    jwks: https://sso.place.com/oauth2/v1/keys
    registration: https://sso.place.com/oauth2/v1/clients
    revocation: https://sso.place.com/oauth2/v1/revoke
    token: https://sso.place.com/oauth2/v1/token
    userinfo: https://sso.place.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  issuer: https://sso.place.com
  name: PLACE SSO (OpenID Connect)
  openIdConnectUrl: https://sso.place.com/.well-known/openid-configuration
  sources:
  - well-known/place-sso-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://sso.place.com/oauth2/default
  name: PLACE SSO custom authorization server ("default")
  observed_use: learn.place.com redirects unauthenticated visitors to https://sso.place.com/oauth2/default/v1/authorize with scope "openid profile email".
  openIdConnectUrl: https://sso.place.com/oauth2/default/.well-known/openid-configuration
  sources:
  - well-known/place-sso-default-openid-configuration.json
  type: openIdConnect
- code_challenge_methods:
  - S256
  dpop_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://hub.place.com/oauth2/v1/authorize
    device_authorization: https://hub.place.com/oauth2/v1/device/authorize
    end_session: https://hub.place.com/oauth2/v1/logout
    introspection: https://hub.place.com/oauth2/v1/introspect
    jwks: https://hub.place.com/oauth2/v1/keys
    pushed_authorization_request: https://hub.place.com/oauth2/v1/par
    registration: https://hub.place.com/oauth2/v1/clients
    revocation: https://hub.place.com/oauth2/v1/revoke
    token: https://hub.place.com/oauth2/v1/token
    userinfo: https://hub.place.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  issuer: https://hub.place.com
  name: PLACE identity hub
  openIdConnectUrl: https://hub.place.com/.well-known/openid-configuration
  sources:
  - well-known/place-hub-openid-configuration.json
  type: openIdConnect
slug: place-authentication
source_filename: place-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: well-known/place-sso-openid-configuration.json, well-known/place-hub-openid-configuration.json\nscope_of_this_file: >-\n  PLACE publishes no product API, so there is no OpenAPI securityScheme set to derive\n  from. What follows is the authentication surface PLACE actually exposes publicly:\n  the OpenID Connect / OAuth 2.0 metadata served from its own single-sign-on hosts.\n  It describes how humans and applications sign in to the PLACE platform — it is NOT\n  evidence of a consumable product API.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, deviceCode, ciba]\n  pkce: [S256]\n  dpop_supported: true\n  mtls_supported: false\n  identity_vendor: Okta\nschemes:\n- name: PLACE SSO (OpenID Connect)\n  type: openIdConnect\n  issuer: https://sso.place.com\n  openIdConnectUrl: https://sso.place.com/.well-known/openid-configuration\n  endpoints:\n \
  \   authorization: https://sso.place.com/oauth2/v1/authorize\n    token: https://sso.place.com/oauth2/v1/token\n    userinfo: https://sso.place.com/oauth2/v1/userinfo\n    jwks: https://sso.place.com/oauth2/v1/keys\n    introspection: https://sso.place.com/oauth2/v1/introspect\n    revocation: https://sso.place.com/oauth2/v1/revoke\n    end_session: https://sso.place.com/oauth2/v1/logout\n    device_authorization: https://sso.place.com/oauth2/v1/device/authorize\n    registration: https://sso.place.com/oauth2/v1/clients\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [S256]\n  sources: [well-known/place-sso-openid-configuration.json]\n- name: PLACE SSO custom authorization server (\"default\")\n  type: openIdConnect\n  issuer: https://sso.place.com/oauth2/default\n\
  \  openIdConnectUrl: https://sso.place.com/oauth2/default/.well-known/openid-configuration\n  observed_use: >-\n    learn.place.com redirects unauthenticated visitors to\n    https://sso.place.com/oauth2/default/v1/authorize with scope \"openid profile email\".\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  code_challenge_methods: [S256]\n  sources: [well-known/place-sso-default-openid-configuration.json]\n- name: PLACE identity hub\n  type: openIdConnect\n  issuer: https://hub.place.com\n  openIdConnectUrl: https://hub.place.com/.well-known/openid-configuration\n  endpoints:\n    authorization: https://hub.place.com/oauth2/v1/authorize\n    token: https://hub.place.com/oauth2/v1/token\n    userinfo: https://hub.place.com/oauth2/v1/userinfo\n    jwks: https://hub.place.com/oauth2/v1/keys\n    introspection: https://hub.place.com/oauth2/v1/introspect\n    revocation: https://hub.place.com/oauth2/v1/revoke\n    end_session:\
  \ https://hub.place.com/oauth2/v1/logout\n    pushed_authorization_request: https://hub.place.com/oauth2/v1/par\n    device_authorization: https://hub.place.com/oauth2/v1/device/authorize\n    registration: https://hub.place.com/oauth2/v1/clients\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba']\n  code_challenge_methods: [S256]\n  dpop_signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n  sources: [well-known/place-hub-openid-configuration.json]\nnot_found:\n  api_keys: no public API-key issuance surface is published\n  mutual_tls: not advertised in any discovery document\n  developer_credentials: >-\n    Dynamic client registration endpoints exist (Okta default) but PLACE publishes no\n    developer program, so no third party can obtain credentials for a product API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/place/refs/heads/main/authentication/place-authentication.yml
summary_line: openIdConnect/oauth2 · 3 schemes
tags:
- Company
- Real-Estate
- Property Technology
- PropTech
- CRM
- Transaction Management
- Brokerage
- MLS
- Mortgage
- Title and Escrow
- Business Services
- Identity
---
