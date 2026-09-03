---
api_key_in: []
api_specs:
- filename: aol-oauth2-api-openapi.yml
  format: yaml
  label: AOL OAuth2 API
  slug: aol-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-oauth2-api-openapi.yml
- filename: aol-openid-connect-api-openapi.yml
  format: yaml
  label: AOL OpenID Connect API
  slug: aol-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-openid-connect-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: probed
name: Aol Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AOL secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AOL
provider_slug: aol
scheme_count: 4
schemes:
- flows:
  - authorizationUrl: https://api.login.aol.com/oauth2/request_auth
    flow: authorizationCode
    refreshUrl: https://api.login.aol.com/oauth2/get_token
    scopes: 4
    tokenUrl: https://api.login.aol.com/oauth2/get_token
  name: oauth2
  sources:
  - https://api.login.aol.com/.well-known/openid-configuration
  type: oauth2
- name: openIdConnect
  openIdConnectUrl: https://api.login.aol.com/.well-known/openid-configuration
  sources:
  - https://api.login.aol.com/.well-known/openid-configuration
  type: openIdConnect
- description: client_secret_basic — HTTP Basic with base64-encoded `client_id:client_secret` at the token endpoint.
  name: basicAuth
  scheme: basic
  sources:
  - https://api.login.aol.com/.well-known/openid-configuration
  - openapi/aol-oauth2-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer access token presented to the userinfo endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aol-openid-connect-api-openapi.yml
  type: http
slug: aol-authentication
source_filename: aol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://api.login.aol.com/.well-known/openid-configuration\ndocs: https://developer.yahoo.com/oauth2/guide/openid_connect/\nnote: >-\n  Upgraded from derived to probed. The baseline was derived from this repo's\n  OpenAPI securitySchemes, which name the legacy Yahoo identity host. AOL runs\n  its OWN OpenID Connect provider at api.login.aol.com and publishes a full\n  discovery document there whose issuer is \"https://api.login.aol.com\" — the\n  values below are read from that document, not from the spec. The Yahoo host\n  is retained as a sibling deployment of the same Oath-era identity platform.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  oauth2_flows:\n  - authorizationCode\n  provider_type: OpenID Connect Provider (OpenID Connect Discovery 1.0)\n  issuer: https://api.login.aol.com\n  mfa_signalled: true\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://api.login.aol.com/oauth2/request_auth\n    tokenUrl: https://api.login.aol.com/oauth2/get_token\n    refreshUrl: https://api.login.aol.com/oauth2/get_token\n    scopes: 4\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.login.aol.com/.well-known/openid-configuration\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    client_secret_basic — HTTP Basic with base64-encoded `client_id:client_secret`\n    at the token endpoint.\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n  - openapi/aol-oauth2-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer access token presented to the userinfo endpoint.\n  sources:\n  - openapi/aol-openid-connect-api-openapi.yml\nendpoints:\n  issuer: https://api.login.aol.com\n\
  \  authorization: https://api.login.aol.com/oauth2/request_auth\n  token: https://api.login.aol.com/oauth2/get_token\n  userinfo: https://api.login.aol.com/openid/v1/userinfo\n  jwks: https://api.login.aol.com/openid/v1/certs\n  introspection: https://api.login.aol.com/oauth2/introspect\n  revocation: https://api.login.aol.com/oauth2/revoke\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\ngrant_types:\n- authorization_code\n- refresh_token\nresponse_types:\n- code\n- token\n- id_token\n- code token\n- code id_token\n- token id_token\n- code token id_token\nresponse_modes:\n- query\nid_token_signing_algs:\n- ES256\n- RS256\nsubject_types:\n- public\nacr_values:\n- AAL1\n- AAL2\nclaims:\n- aud\n- auth_time\n- birthdate\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- iss\n- locale\n- name\n- sub\nnot_supported:\n  claims_parameter: false\n  request_parameter: false\n  request_uri_parameter: false\n  note: >-\n    Signed/pushed request objects\
  \ (RFC 9101) and the OIDC `claims` request\n    parameter are explicitly unsupported per the discovery document.\nevidence:\n- url: https://api.login.aol.com/.well-known/openid-configuration\n  status: 200\n  content_type: application/json\n  fetched: '2026-09-02'\n- url: https://api.login.aol.com/openid/v1/certs\n  status: 200\n  content_type: application/json\n  fetched: '2026-09-02'\n  note: JWKS served anonymously; RSA/RS256 signing keys present.\n- url: https://api.login.aol.com/oauth2/introspect\n  status: 403\n  fetched: '2026-09-02'\n  note: Introspection endpoint exists per discovery but rejects anonymous callers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/authentication/aol-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Digital Media
- News
- Entertainment
- Advertising
- Identity
- OpenID Connect
- Authentication
- Email
- Consumer Internet
- Fortune 1000
---
