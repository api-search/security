---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Tegus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- refreshToken
- deviceCode
- tokenExchange
overview: Tegus secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, refreshToken, deviceCode, and tokenExchange flow(s).
provider_name: Tegus
provider_slug: tegus
scheme_count: 2
schemes:
- issuer: https://auth.tegus.com/
  name: TegusOpenIDConnect
  openIdConnectUrl: https://auth.tegus.com/.well-known/openid-configuration
  sources:
  - well-known/tegus-openid-configuration.json
  type: openIdConnect
- backchannel_logout_supported: true
  code_challenge_methods:
  - S256
  - plain
  dpop_signing_algs:
  - ES256
  dynamic_client_registration: true
  endpoints:
    authorization: https://auth.tegus.com/authorize
    backchannel_authentication: https://auth.tegus.com/bc-authorize
    device_authorization: https://auth.tegus.com/oauth/device/code
    global_token_revocation: https://auth.tegus.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.tegus.com/.well-known/jwks.json
    mfa_challenge: https://auth.tegus.com/mfa/challenge
    registration: https://auth.tegus.com/oidc/register
    revocation: https://auth.tegus.com/oauth/revoke
    token: https://auth.tegus.com/oauth/token
    userinfo: https://auth.tegus.com/userinfo
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.tegus.com/
  name: TegusOAuth2
  request_parameter_supported: false
  request_uri_parameter_supported: false
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/tegus-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: oauth2
slug: tegus-authentication
source_filename: tegus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://auth.tegus.com/.well-known/openid-configuration\ndocs: https://auth.tegus.com/.well-known/openid-configuration\nnote: >-\n  Derived entirely from the live OpenID Connect Discovery and RFC 8414 metadata served\n  by auth.tegus.com. There is no published Tegus API reference to corroborate against —\n  the Tegus developer hub (tegus.readme.io) now 302s to /inactive and the product API\n  hosts no longer resolve. This profile therefore describes the identity layer of the\n  Tegus platform, not a product API contract.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - refreshToken\n  - deviceCode\n  - tokenExchange\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  mtls: false\n  api_key_in: []\nschemes:\n- name: TegusOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.tegus.com/.well-known/openid-configuration\n\
  \  issuer: https://auth.tegus.com/\n  sources:\n  - well-known/tegus-openid-configuration.json\n- name: TegusOAuth2\n  type: oauth2\n  issuer: https://auth.tegus.com/\n  endpoints:\n    authorization: https://auth.tegus.com/authorize\n    token: https://auth.tegus.com/oauth/token\n    userinfo: https://auth.tegus.com/userinfo\n    jwks: https://auth.tegus.com/.well-known/jwks.json\n    revocation: https://auth.tegus.com/oauth/revoke\n    registration: https://auth.tegus.com/oidc/register\n    device_authorization: https://auth.tegus.com/oauth/device/code\n    backchannel_authentication: https://auth.tegus.com/bc-authorize\n    mfa_challenge: https://auth.tegus.com/mfa/challenge\n    global_token_revocation: https://auth.tegus.com/oauth/global-token-revocation/connection/{connectionName}\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  response_modes:\n  - query\n  - fragment\n  - form_post\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs:\n  - RS256\n  - RS384\n  - PS256\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\n  code_challenge_methods:\n  - S256\n  - plain\n  dynamic_client_registration: true\n  backchannel_logout_supported: true\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  sources:\n  - well-known/tegus-oauth-authorization-server.json\nobservations:\n\
  - id: implicit-grant-enabled\n  detail: >-\n    The implicit grant and the resource-owner password grant are both advertised in\n    grant_types_supported. Both are discouraged by OAuth 2.1 / BCP 225.\n- id: plain-pkce-allowed\n  detail: >-\n    code_challenge_methods_supported includes \"plain\" alongside S256.\n- id: hs256-id-tokens\n  detail: >-\n    id_token_signing_alg_values_supported includes the symmetric HS256 alongside RS256/PS256.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://auth.tegus.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegus/refs/heads/main/authentication/tegus-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Investment Research
- Expert Networks
- Market Intelligence
- Financial Data
- Transcripts
- Private Markets
- Equity Research
- OpenID Connect
- Acquired
---
