---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Houm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Houm declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Houm
provider_slug: houm
scheme_count: 1
schemes:
- backchannel_logout_supported: true
  endpoints:
    authorization: https://auth.houm.com/authorize
    device_authorization: https://auth.houm.com/oauth/device/code
    jwks: https://auth.houm.com/.well-known/jwks.json
    mfa_challenge: https://auth.houm.com/mfa/challenge
    registration: https://auth.houm.com/oidc/register
    revocation: https://auth.houm.com/oauth/revoke
    token: https://auth.houm.com/oauth/token
    userinfo: https://auth.houm.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - RS256
  - PS256
  - HS256
  issuer: https://auth.houm.com/
  mfa: true
  name: openIdConnect
  openIdConnectUrl: https://auth.houm.com/.well-known/openid-configuration
  pkce_methods:
  - S256
  - plain
  provider: Auth0 (custom domain)
  request_uri_parameter_supported: false
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: houm-authentication
source_filename: houm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.houm.com/.well-known/openid-configuration\nname: Houm authentication\nnote: >-\n  Houm publishes no API reference and no OpenAPI, so there are no securitySchemes to derive from.\n  This profile is built entirely from the OpenID Connect discovery document Houm's own Auth0 custom\n  domain serves anonymously at auth.houm.com, saved verbatim in\n  well-known/houm-openid-configuration.json. It describes how Houm authenticates users of its own\n  web and mobile products (houm.com, admin.houm.com — whose CSP frame-src names auth.houm.com and\n  *.auth0.com). It is NOT documentation of a public developer API: no client registration, key\n  issuance, or authorization flow for third parties is published anywhere on Houm's site.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.houm.com/.well-known/openid-configuration\n  issuer: https://auth.houm.com/\n  provider: Auth0 (custom domain)\n\
  \  endpoints:\n    authorization: https://auth.houm.com/authorize\n    token: https://auth.houm.com/oauth/token\n    userinfo: https://auth.houm.com/userinfo\n    jwks: https://auth.houm.com/.well-known/jwks.json\n    revocation: https://auth.houm.com/oauth/revoke\n    registration: https://auth.houm.com/oidc/register\n    device_authorization: https://auth.houm.com/oauth/device/code\n    mfa_challenge: https://auth.houm.com/mfa/challenge\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  -\
  \ token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  pkce_methods:\n  - S256\n  - plain\n  id_token_signing_algs:\n  - RS256\n  - PS256\n  - HS256\n  mfa: true\n  backchannel_logout_supported: true\n  request_uri_parameter_supported: false\ndocs: null\ndocs_note: >-\n  No authentication documentation is published by Houm. help.houm.com is an end-user help centre\n  with no developer or API section, and developers.houm.com does not resolve.\nevidence:\n- url: https://auth.houm.com/.well-known/openid-configuration\n  status: 200\n- url: https://auth.houm.com/.well-known/jwks.json\n  status: 200\n- url: https://help.houm.com/cl\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houm/refs/heads/main/authentication/houm-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real-Estate
- PropTech
- Property Management
- Rentals
- Marketplace
- Latin America
- Chile
- Mexico
- Colombia
---
