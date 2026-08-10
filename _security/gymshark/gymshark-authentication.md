---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gymshark Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- refreshToken
- password
- tokenExchange
overview: Gymshark secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, refreshToken, password, and tokenExchange flow(s).
provider_name: Gymshark
provider_slug: gymshark
scheme_count: 2
schemes:
- issuer: https://auth.gymshark.com/
  name: gymshark-oidc
  openIdConnectUrl: https://auth.gymshark.com/.well-known/openid-configuration
  sources:
  - well-known/gymshark-openid-configuration.json
  type: openIdConnect
  vendor: Auth0
- flows:
  - authorizationUrl: https://auth.gymshark.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.gymshark.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.gymshark.com/oauth/token
  - authorizationUrl: https://auth.gymshark.com/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://auth.gymshark.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.gymshark.com/oauth/token
  issuer: https://auth.gymshark.com/
  name: gymshark-oauth2
  sources:
  - well-known/gymshark-oauth-authorization-server.json
  type: oauth2
slug: gymshark-authentication
source_filename: gymshark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://auth.gymshark.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Gymshark publishes no OpenAPI and no developer authentication documentation, so this\n  profile is read directly from the OpenID Connect Discovery / RFC 8414 metadata that\n  Gymshark's own authorization server publishes anonymously at auth.gymshark.com. It\n  describes how Gymshark customer accounts authenticate across the storefronts and the\n  Gymshark Shop / Gymshark Training mobile apps. It is not a self-serve developer API —\n  there is no published client-registration or partner onboarding path.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - deviceCode\n  - refreshToken\n  - password\n  - tokenExchange\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  mfa: true\n  dynamic_client_registration: true\nschemes:\n- name: gymshark-oidc\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://auth.gymshark.com/.well-known/openid-configuration\n  issuer: https://auth.gymshark.com/\n  vendor: Auth0\n  sources:\n  - well-known/gymshark-openid-configuration.json\n- name: gymshark-oauth2\n  type: oauth2\n  issuer: https://auth.gymshark.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.gymshark.com/authorize\n    tokenUrl: https://auth.gymshark.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.gymshark.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.gymshark.com/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.gymshark.com/oauth/device/code\n    tokenUrl: https://auth.gymshark.com/oauth/token\n  sources:\n  - well-known/gymshark-oauth-authorization-server.json\nendpoints:\n  issuer: https://auth.gymshark.com/\n  authorization: https://auth.gymshark.com/authorize\n  token: https://auth.gymshark.com/oauth/token\n  userinfo: https://auth.gymshark.com/userinfo\n\
  \  jwks: https://auth.gymshark.com/.well-known/jwks.json\n  registration: https://auth.gymshark.com/oidc/register\n  revocation: https://auth.gymshark.com/oauth/revoke\n  device_authorization: https://auth.gymshark.com/oauth/device/code\n  backchannel_authentication: https://auth.gymshark.com/bc-authorize\n  mfa_challenge: https://auth.gymshark.com/mfa/challenge\n  global_token_revocation: https://auth.gymshark.com/oauth/global-token-revocation/connection/{connectionName}\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\nresponse_types_supported:\n- code\n- token\n- id_token\n- code\
  \ token\n- code id_token\n- token id_token\n- code token id_token\nresponse_modes_supported:\n- query\n- fragment\n- form_post\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\ntoken_endpoint_auth_signing_alg_values_supported:\n- RS256\n- RS384\n- PS256\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\ndpop_signing_alg_values_supported:\n- ES256\nsubject_types_supported:\n- public\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\nsession_management:\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\n  backchannel_token_delivery_modes_supported:\n  - poll\nrequest_object_support:\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\nobservations:\n- >-\n  The legacy `password` (resource owner password\
  \ credentials) and `implicit` grants\n  are still advertised alongside authorization_code + PKCE; both are discouraged by\n  OAuth 2.1 and the OAuth 2.0 Security BCP (RFC 9700).\n- >-\n  `code_challenge_methods_supported` still lists `plain` in addition to `S256`; `S256`\n  is the only method OAuth 2.1 permits.\n- >-\n  `id_token_signing_alg_values_supported` still lists the symmetric `HS256` alongside\n  `RS256`/`PS256`.\n- >-\n  DPoP (RFC 9449) sender-constrained tokens are supported (ES256), as is RFC 8693\n  token exchange and RFC 7591 dynamic client registration.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://auth.gymshark.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gymshark/refs/heads/main/authentication/gymshark-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fitness
- Consumer
- Direct To Consumer
- Identity
- OpenID Connect
---
