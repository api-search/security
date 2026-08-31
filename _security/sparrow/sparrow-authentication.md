---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sparrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sparrow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sparrow
provider_slug: sparrow
scheme_count: 1
schemes:
- backchannel_logout:
    session_supported: true
    supported: true
  dpop:
    signing_alg_values:
    - ES256
    supported: true
  endpoints:
    authorization: https://login.trysparrow.com/authorize
    backchannel_authentication: https://login.trysparrow.com/bc-authorize
    device_authorization: https://login.trysparrow.com/oauth/device/code
    dynamic_registration: https://login.trysparrow.com/oidc/register
    jwks: https://login.trysparrow.com/.well-known/jwks.json
    revocation: https://login.trysparrow.com/oauth/revoke
    token: https://login.trysparrow.com/oauth/token
    userinfo: https://login.trysparrow.com/userinfo
  federation:
    note: SAML SSO is offered to enterprise customers via trysparrow-samlidp.us.auth0.com (named in the app.trysparrow.com Content-Security-Policy) and referenced on the Sparrow security page.
    saml: true
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  mfa:
    challenge_endpoint: https://login.trysparrow.com/mfa/challenge
    grant_types:
    - http://auth0.com/oauth/grant-type/mfa-oob
    - http://auth0.com/oauth/grant-type/mfa-otp
    - http://auth0.com/oauth/grant-type/mfa-recovery-code
    supported: true
  name: sparrow_oidc
  openIdConnectUrl: https://login.trysparrow.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  response_types:
  - code
  - token
  - id_token
  - code id_token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: sparrow-authentication
source_filename: sparrow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://login.trysparrow.com/.well-known/openid-configuration\ndocs: https://sparrow.com/security/\nnote: >-\n  Sparrow publishes no developer API and no API-key or OAuth programme for third parties. What IS\n  anonymously published is the authentication surface of Sparrow's own web application: an OpenID\n  Connect provider on Sparrow's custom domain login.trysparrow.com (an Auth0 tenant — the app's CSP\n  names trysparrow-samlidp.us.auth0.com as a permitted frame source, and Sparrow's security page\n  documents SAML SSO for enterprise customers). This profile is derived entirely from the\n  anonymously-served discovery document; it describes how humans and Sparrow's own SPA sign in, NOT\n  a partner-facing authorization server. No client registration is open to the public.\nsurface: end-user and customer application sign-in\nissuer: https://login.trysparrow.com/\nprovider: Auth0 (custom domain on trysparrow.com)\nschemes:\n\
  - name: sparrow_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.trysparrow.com/.well-known/openid-configuration\n  endpoints:\n    authorization: https://login.trysparrow.com/authorize\n    token: https://login.trysparrow.com/oauth/token\n    userinfo: https://login.trysparrow.com/userinfo\n    jwks: https://login.trysparrow.com/.well-known/jwks.json\n    revocation: https://login.trysparrow.com/oauth/revoke\n    device_authorization: https://login.trysparrow.com/oauth/device/code\n    backchannel_authentication: https://login.trysparrow.com/bc-authorize\n    dynamic_registration: https://login.trysparrow.com/oidc/register\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  - token\n  - id_token\n  - code id_token\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  dpop:\n    supported: true\n    signing_alg_values:\n    - ES256\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  mfa:\n    supported: true\n    challenge_endpoint: https://login.trysparrow.com/mfa/challenge\n    grant_types:\n    - http://auth0.com/oauth/grant-type/mfa-oob\n    - http://auth0.com/oauth/grant-type/mfa-otp\n    - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  backchannel_logout:\n    supported: true\n    session_supported: true\n  federation:\n    saml: true\n    note: >-\n      SAML SSO is offered to enterprise customers via trysparrow-samlidp.us.auth0.com (named in the\n      app.trysparrow.com Content-Security-Policy) and referenced on the Sparrow security page.\napi_key_auth:\n  published: false\n  note: No public API key programme, developer portal, or key-issuance flow is published.\n\
  evidence:\n- url: https://login.trysparrow.com/.well-known/openid-configuration\n  status: 200\n- url: https://login.trysparrow.com/.well-known/jwks.json\n  status: 200\n- url: https://api.trysparrow.com/.well-known/oauth-protected-resource\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparrow/refs/heads/main/authentication/sparrow-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Leave Management
- Human Resources
- HR Tech
- Payroll
- Compliance
- Employee Benefits
- Absence Management
- Software-as-a-Service
---
