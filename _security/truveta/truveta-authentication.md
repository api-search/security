---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: Truveta publishes no OpenAPI, so this profile is not derived from a spec. It is read directly from the OpenID Connect discovery document Truveta's own Auth0 identity tenant serves anonymously at login.truveta.com. This is the authentication surface in front of Truveta Studio; there is no separately documented public API to authenticate against.
kind: authentication
layout: security
method: searched
name: Truveta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
overview: Truveta secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, and tokenExchange flow(s).
provider_name: Truveta
provider_slug: truveta
scheme_count: 2
schemes:
- issuer: https://login.truveta.com/
  name: TruvetaOIDC
  openIdConnectUrl: https://login.truveta.com/.well-known/openid-configuration
  sources:
  - well-known/truveta-openid-configuration.json
  type: openIdConnect
- backchannel_logout_supported: true
  code_challenge_methods:
  - S256
  - plain
  dpop_supported: true
  endpoints:
    authorization: https://login.truveta.com/authorize
    backchannel_authentication: https://login.truveta.com/bc-authorize
    device_authorization: https://login.truveta.com/oauth/device/code
    end_session: https://login.truveta.com/oidc/logout
    jwks: https://login.truveta.com/.well-known/jwks.json
    mfa_challenge: https://login.truveta.com/mfa/challenge
    registration: https://login.truveta.com/oidc/register
    revocation: https://login.truveta.com/oauth/revoke
    token: https://login.truveta.com/oauth/token
    userinfo: https://login.truveta.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
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
  name: TruvetaOAuth2
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/truveta-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
slug: truveta-authentication
source_filename: truveta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://login.truveta.com/.well-known/openid-configuration\ndocs: https://studio.truveta.com/\ndescription: >-\n  Truveta publishes no OpenAPI, so this profile is not derived from a spec. It\n  is read directly from the OpenID Connect discovery document Truveta's own\n  Auth0 identity tenant serves anonymously at login.truveta.com. This is the\n  authentication surface in front of Truveta Studio; there is no separately\n  documented public API to authenticate against.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken, tokenExchange]\n  identity_provider: Auth0\n  pkce: true\n  mfa: true\nschemes:\n  - name: TruvetaOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://login.truveta.com/.well-known/openid-configuration\n    issuer: https://login.truveta.com/\n    sources: [well-known/truveta-openid-configuration.json]\n  - name:\
  \ TruvetaOAuth2\n    type: oauth2\n    sources: [well-known/truveta-openid-configuration.json]\n    endpoints:\n      authorization: https://login.truveta.com/authorize\n      token: https://login.truveta.com/oauth/token\n      device_authorization: https://login.truveta.com/oauth/device/code\n      userinfo: https://login.truveta.com/userinfo\n      revocation: https://login.truveta.com/oauth/revoke\n      registration: https://login.truveta.com/oidc/register\n      end_session: https://login.truveta.com/oidc/logout\n      jwks: https://login.truveta.com/.well-known/jwks.json\n      backchannel_authentication: https://login.truveta.com/bc-authorize\n      mfa_challenge: https://login.truveta.com/mfa/challenge\n    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \      - http://auth0.com/oauth/grant-type/password-realm\n      - http://auth0.com/oauth/grant-type/passwordless/otp\n      - http://auth0.com/oauth/grant-type/mfa-oob\n      - http://auth0.com/oauth/grant-type/mfa-otp\n      - http://auth0.com/oauth/grant-type/mfa-recovery-code\n    response_types: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n    code_challenge_methods: [S256, plain]\n    id_token_signing_algs: [HS256, RS256, PS256]\n    dpop_supported: true\n    backchannel_logout_supported: true\n    subject_types: [public]\nclaims_supported:\n  - aud\n  - auth_time\n  - created_at\n  - email\n  - email_verified\n  - exp\n  - family_name\n  - given_name\n  - iat\n  - identities\n  - iss\n  - name\n  - nickname\n  - phone_number\n  - picture\n  - sub\nnotes:\n  - >-\n    Access is customer-only. studio.truveta.com issues an HTTP 302 into the\n\
  \    Auth0 universal login at login.truveta.com; there is no self-serve sign-up\n    and no anonymous developer tier.\n  - >-\n    No API key, HTTP basic, HTTP bearer, or mutual-TLS scheme is documented\n    anywhere on Truveta's public surface.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://login.truveta.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truveta/refs/heads/main/authentication/truveta-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Data
- Electronic Health Records
- Real-World Evidence
- Clinical Research
- Life Sciences
- Genomics
- Analytics
- Artificial Intelligence
- Data Platform
---
