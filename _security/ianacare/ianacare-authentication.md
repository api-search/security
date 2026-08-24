---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ianacare Authentication
name_suffix: Authentication
oauth_flows: []
overview: ianacare declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ianacare
provider_slug: ianacare
scheme_count: 3
schemes:
- description: OpenID Connect discovery served from ianacare's own auth host. Backs the ianacare mobile apps (com.ianacare.iana / com.ianacare.ianacare) and the app.ianacare.com web client.
  endpoints:
    authorization: https://auth.ianacare.com/authorize
    backchannel_authentication: https://auth.ianacare.com/bc-authorize
    device_authorization: https://auth.ianacare.com/oauth/device/code
    global_token_revocation: https://auth.ianacare.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.ianacare.com/.well-known/jwks.json
    mfa_challenge: https://auth.ianacare.com/mfa/challenge
    registration: https://auth.ianacare.com/oidc/register
    revocation: https://auth.ianacare.com/oauth/revoke
    token: https://auth.ianacare.com/oauth/token
    userinfo: https://auth.ianacare.com/userinfo
  id: oidc
  openIdConnectUrl: https://auth.ianacare.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 authorization server (RFC 8414 metadata identical to the OIDC document).
  dpop_signing_algs:
  - ES256
  flows:
    authorization_code:
      authorizationUrl: https://auth.ianacare.com/authorize
      code_challenge_methods:
      - S256
      - plain
      pkce: true
      tokenUrl: https://auth.ianacare.com/oauth/token
    client_credentials:
      tokenUrl: https://auth.ianacare.com/oauth/token
    device_code:
      deviceAuthorizationUrl: https://auth.ianacare.com/oauth/device/code
    refresh_token:
      tokenUrl: https://auth.ianacare.com/oauth/token
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
  id: oauth2
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
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
  type: oauth2
- bearerFormat: JWT
  description: Resource-server side. iana.ianacare.com answers an unauthenticated request with HTTP 401 and {"error":{"code":"auth_denied","message":"Missing bearer token", "request_id":"..."}} — the tokens are the JWTs minted by auth.ianacare.com above.
  id: bearer
  observed:
    body: '{"error":{"code":"auth_denied","message":"Missing bearer token","request_id":"<uuid>"}}'
    status: 401
    url: https://iana.ianacare.com/api/v1
  scheme: bearer
  type: http
slug: ianacare-authentication
source_filename: ianacare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.ianacare.com/.well-known/openid-configuration\nnote: >-\n  Derived entirely from documents ianacare serves, not from any published developer\n  documentation — ianacare publishes no developer portal, no API reference and no\n  OpenAPI. The OIDC discovery document at auth.ianacare.com is real and first-party\n  (auth.ianacare.com is ianacare's own hostname, CNAMEd to its Auth0 tenant\n  prod-env-ianacare-cd-wcczcfxw9amotowp.edge.tenants.us.auth0.com), and the bearer\n  challenge below was observed live against iana.ianacare.com.\nidentity_provider:\n  vendor: Auth0\n  custom_domain: auth.ianacare.com\n  issuer: https://auth.ianacare.com/\n  evidence: dig CNAME auth.ianacare.com -> prod-env-ianacare-cd-wcczcfxw9amotowp.edge.tenants.us.auth0.com\nschemes:\n- id: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.ianacare.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect discovery\
  \ served from ianacare's own auth host. Backs the ianacare\n    mobile apps (com.ianacare.iana / com.ianacare.ianacare) and the app.ianacare.com\n    web client.\n  endpoints:\n    authorization: https://auth.ianacare.com/authorize\n    token: https://auth.ianacare.com/oauth/token\n    userinfo: https://auth.ianacare.com/userinfo\n    jwks: https://auth.ianacare.com/.well-known/jwks.json\n    revocation: https://auth.ianacare.com/oauth/revoke\n    registration: https://auth.ianacare.com/oidc/register\n    device_authorization: https://auth.ianacare.com/oauth/device/code\n    backchannel_authentication: https://auth.ianacare.com/bc-authorize\n    mfa_challenge: https://auth.ianacare.com/mfa/challenge\n    global_token_revocation: https://auth.ianacare.com/oauth/global-token-revocation/connection/{connectionName}\n- id: oauth2\n  type: oauth2\n  description: OAuth 2.0 authorization server (RFC 8414 metadata identical to the OIDC document).\n  flows:\n    authorization_code:\n      authorizationUrl:\
  \ https://auth.ianacare.com/authorize\n      tokenUrl: https://auth.ianacare.com/oauth/token\n      pkce: true\n      code_challenge_methods: [S256, plain]\n    client_credentials:\n      tokenUrl: https://auth.ianacare.com/oauth/token\n    device_code:\n      deviceAuthorizationUrl: https://auth.ianacare.com/oauth/device/code\n    refresh_token:\n      tokenUrl: https://auth.ianacare.com/oauth/token\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n\
  \  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs: [RS256, RS384, PS256]\n  id_token_signing_algs: [HS256, RS256, PS256]\n  dpop_signing_algs: [ES256]\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  response_modes: [query, fragment, form_post]\n  subject_types: [public]\n- id: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Resource-server side. iana.ianacare.com answers an unauthenticated request with\n    HTTP 401 and {\"error\":{\"code\":\"auth_denied\",\"message\":\"Missing bearer token\",\n    \"request_id\":\"...\"}} — the tokens are the JWTs minted by auth.ianacare.com above.\n  observed:\n    url: https://iana.ianacare.com/api/v1\n    status: 401\n    body: '{\"error\":{\"code\":\"auth_denied\",\"message\":\"Missing bearer token\",\"request_id\":\"<uuid>\"}}'\nmfa:\n  supported: true\n  evidence: mfa_challenge_endpoint present in the discovery\
  \ document\n  factors_documented: false\ndynamic_client_registration:\n  supported: true\n  endpoint: https://auth.ianacare.com/oidc/register\n  note: >-\n    RFC 7591 registration endpoint is advertised in discovery. Not tested — no anonymous\n    registration attempt was made against a production tenant.\ngaps:\n- No public developer documentation describes how a third party would obtain a client_id.\n- No audience/API identifier is published, so the scopes an access token can carry for\n  the iana.ianacare.com resource server are not discoverable anonymously.\n- api.ianacare.com returns HTTP 403 on every path, so its auth model cannot be observed.\nx-evidence:\n  fetched: '2026-08-22'\n  urls:\n  - url: https://auth.ianacare.com/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.ianacare.com/.well-known/jwks.json\n    status: 200\n  - url: https://iana.ianacare.com/api/v1\n    status: 401\n  - url: https://api.ianacare.com/\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ianacare/refs/heads/main/authentication/ianacare-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Health Care
- Caregiving
- Employee Benefits
- Digital Health
- Care Navigation
- Health Plans
- Mobile Application
- Identity
---
