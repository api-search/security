---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Honey Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- refreshToken
- password
overview: Honey Insurance secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, refreshToken, and password flow(s).
provider_name: Honey Insurance
provider_slug: honey-insurance
scheme_count: 1
schemes:
- backchannel_logout_session_supported: true
  backchannel_logout_supported: true
  backchannel_token_delivery_modes_supported:
  - poll
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://auth.honeyinsurance.com/authorize
    backchannel_authentication: https://auth.honeyinsurance.com/bc-authorize
    device_authorization: https://auth.honeyinsurance.com/oauth/device/code
    global_token_revocation: https://auth.honeyinsurance.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.honeyinsurance.com/.well-known/jwks.json
    mfa_challenge: https://auth.honeyinsurance.com/mfa/challenge
    registration: https://auth.honeyinsurance.com/oidc/register
    revocation: https://auth.honeyinsurance.com/oauth/revoke
    token: https://auth.honeyinsurance.com/oauth/token
    userinfo: https://auth.honeyinsurance.com/userinfo
  grant_types_supported:
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
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.honeyinsurance.com/
  mfa: true
  name: Auth0OIDC
  openIdConnectUrl: https://auth.honeyinsurance.com/.well-known/openid-configuration
  request_parameter_supported: false
  request_uri_parameter_supported: false
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  source: well-known/honey-insurance-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: honey-insurance-authentication
source_filename: honey-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.honeyinsurance.com/.well-known/openid-configuration\ndocs: null\ndeveloper_credentials: false\nnote: >-\n  Honey Insurance issues no developer API credentials. There is no developer\n  portal, no key-issuance page and no client-registration path documented for\n  third parties. The one authentication surface that is anonymously\n  discoverable is an Auth0 custom-domain tenant used for consumer \"My account\"\n  sign-in; its metadata is captured verbatim in\n  well-known/honey-insurance-openid-configuration.json. The private backend at\n  api.honeyinsurance.com publishes no auth documentation and denies all\n  anonymous requests with HTTP 403.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  audience: end-user consumer accounts only\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  - password\n  api_key_in: []\n  mutual_tls: false\nschemes:\n-\
  \ name: Auth0OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.honeyinsurance.com/.well-known/openid-configuration\n  issuer: https://auth.honeyinsurance.com/\n  source: well-known/honey-insurance-openid-configuration.json\n  endpoints:\n    authorization: https://auth.honeyinsurance.com/authorize\n    token: https://auth.honeyinsurance.com/oauth/token\n    userinfo: https://auth.honeyinsurance.com/userinfo\n    jwks: https://auth.honeyinsurance.com/.well-known/jwks.json\n    revocation: https://auth.honeyinsurance.com/oauth/revoke\n    registration: https://auth.honeyinsurance.com/oidc/register\n    device_authorization: https://auth.honeyinsurance.com/oauth/device/code\n    mfa_challenge: https://auth.honeyinsurance.com/mfa/challenge\n    backchannel_authentication: https://auth.honeyinsurance.com/bc-authorize\n    global_token_revocation: https://auth.honeyinsurance.com/oauth/global-token-revocation/connection/{connectionName}\n  grant_types_supported:\n  - client_credentials\n\
  \  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  subject_types_supported:\n  - public\n  dpop_signing_alg_values_supported:\n  - ES256\n  backchannel_token_delivery_modes_supported:\n\
  \  - poll\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  mfa: true\ntokens:\n  format: JWT\n  signing: RS256 / PS256 / HS256 (per Auth0 tenant metadata)\n  pkce: supported (S256)\n  jwks: well-known/honey-insurance-jwks.json\ngaps:\n- No API audience is published, so no access token can be requested for an\n  insurance-domain API.\n- No developer client registration; /oidc/register is the stock Auth0 dynamic\n  registration endpoint and is not documented for third parties.\n- No insurance-domain scopes exist — see scopes/honey-insurance-scopes.yml.\n- The production API host (api.honeyinsurance.com) documents no scheme at all.\nrelated:\n  scopes: scopes/honey-insurance-scopes.yml\n  well_known: well-known/honey-insurance-well-known.yml\n  conformance: conformance/honey-insurance-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honey-insurance/refs/heads/main/authentication/honey-insurance-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Insurance
- Australia
- Insurtech
- Home Insurance
- Property and Casualty
- Personal Lines
- Direct to Consumer
- Embedded Insurance
- Smart Home
- Claims
- Underwriting
---
