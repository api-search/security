---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Mainstreet Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- refresh_token
- implicit
- password
- device_code
overview: MainStreet secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, refresh_token, implicit, password, and device_code flow(s).
provider_name: MainStreet
provider_slug: mainstreet
scheme_count: 1
schemes:
- authorization_grant_profiles:
  - urn:ietf:params:oauth:grant-profile:id-jag
  backchannel_logout_session_supported: true
  backchannel_logout_supported: true
  backchannel_token_delivery_modes:
  - poll
  code_challenge_methods:
  - S256
  - plain
  dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://login.mainstreet.com/authorize
    backchannel_authentication: https://login.mainstreet.com/bc-authorize
    device_authorization: https://login.mainstreet.com/oauth/device/code
    global_token_revocation: https://login.mainstreet.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://login.mainstreet.com/.well-known/jwks.json
    mfa_challenge: https://login.mainstreet.com/mfa/challenge
    registration: https://login.mainstreet.com/oidc/register
    revocation: https://login.mainstreet.com/oauth/revoke
    token: https://login.mainstreet.com/oauth/token
    userinfo: https://login.mainstreet.com/userinfo
  grant_types:
  - client_credentials
  - authorization_code
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
  - HS256
  - RS256
  - PS256
  issuer: https://login.mainstreet.com/
  name: MainStreet OIDC (Auth0 tenant)
  openIdConnectUrl: https://login.mainstreet.com/.well-known/openid-configuration
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
  - well-known/mainstreet-openid-configuration.json
  - well-known/mainstreet-oauth-authorization-server.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
slug: mainstreet-authentication
source_filename: mainstreet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://login.mainstreet.com/.well-known/openid-configuration\ndocs: https://login.mainstreet.com/.well-known/openid-configuration\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - device_code\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  mfa: true\n  note: >-\n    MainStreet publishes no public product API and no OpenAPI document. The only\n    machine-readable authentication contract it serves is the OIDC/OAuth 2.0\n    discovery pair on its Auth0-hosted identity domain, which backs sign-in to the\n    client portal (dashboard.mainstreet.com) and the bookkeeping app\n    (books.mainstreet.com). This profile is transcribed from that discovery\n    document — nothing here is inferred.\nschemes:\n- name: MainStreet OIDC (Auth0 tenant)\n  type: openIdConnect\n  openIdConnectUrl: https://login.mainstreet.com/.well-known/openid-configuration\n\
  \  issuer: https://login.mainstreet.com/\n  endpoints:\n    authorization: https://login.mainstreet.com/authorize\n    token: https://login.mainstreet.com/oauth/token\n    userinfo: https://login.mainstreet.com/userinfo\n    jwks: https://login.mainstreet.com/.well-known/jwks.json\n    revocation: https://login.mainstreet.com/oauth/revoke\n    registration: https://login.mainstreet.com/oidc/register\n    device_authorization: https://login.mainstreet.com/oauth/device/code\n    backchannel_authentication: https://login.mainstreet.com/bc-authorize\n    mfa_challenge: https://login.mainstreet.com/mfa/challenge\n    global_token_revocation: https://login.mainstreet.com/oauth/global-token-revocation/connection/{connectionName}\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  -\
  \ http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  authorization_grant_profiles:\n  - urn:ietf:params:oauth:grant-profile:id-jag\n  backchannel_token_delivery_modes:\n  - poll\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  response_modes:\n  - query\n  - fragment\n  - form_post\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs:\n  - RS256\n  - RS384\n  - PS256\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  code_challenge_methods:\n  - S256\n  - plain\n  dpop_signing_algs:\n  - ES256\n  subject_types:\n  - public\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported:\
  \ true\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  sources:\n  - well-known/mainstreet-openid-configuration.json\n  - well-known/mainstreet-oauth-authorization-server.json\nhuman_auth:\n  login_url: https://login.mainstreet.com/u/login\n  sign_up_url: https://dashboard.mainstreet.com/welcome\n  note: >-\n    End users authenticate through the hosted Auth0 universal login; there is no\n    published developer API key, personal access token, or partner credential\n    program on MainStreet's public surface.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://login.mainstreet.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mainstreet/refs/heads/main/authentication/mainstreet-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Tax
- Tax Credits
- Accounting
- Financial-Services
- Small Business
- Fintech
- Bookkeeping
- Compliance
- Payroll
---
