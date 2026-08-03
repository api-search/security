---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ambience Healthcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
- jwtBearer
- implicit
- password
overview: Ambience Healthcare secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, tokenExchange, jwtBearer, implicit, and password flow(s).
provider_name: Ambience Healthcare
provider_slug: ambience-healthcare
scheme_count: 2
schemes:
- endpoints:
    authorization: https://auth.ambiencehealthcare.com/authorize
    backchannel_authentication: https://auth.ambiencehealthcare.com/bc-authorize
    device_authorization: https://auth.ambiencehealthcare.com/oauth/device/code
    jwks: https://auth.ambiencehealthcare.com/.well-known/jwks.json
    mfa_challenge: https://auth.ambiencehealthcare.com/mfa/challenge
    registration: https://auth.ambiencehealthcare.com/oidc/register
    revocation: https://auth.ambiencehealthcare.com/oauth/revoke
    token: https://auth.ambiencehealthcare.com/oauth/token
    userinfo: https://auth.ambiencehealthcare.com/userinfo
  issuer: https://auth.ambiencehealthcare.com/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.ambiencehealthcare.com/.well-known/openid-configuration
  sources:
  - well-known/ambience-healthcare-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.ambiencehealthcare.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  - deviceAuthorizationUrl: https://auth.ambiencehealthcare.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  - authorizationUrl: https://auth.ambiencehealthcare.com/authorize
    flow: implicit
    note: advertised in response_types_supported; not recommended, recorded as observed
  grant_types_supported:
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
  name: OAuth2
  sources:
  - well-known/ambience-healthcare-openid-configuration.json
  type: oauth2
slug: ambience-healthcare-authentication
source_filename: ambience-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://auth.ambiencehealthcare.com/.well-known/openid-configuration\ndocs: https://www.ambiencehealthcare.com/informatics\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  - tokenExchange\n  - jwtBearer\n  - implicit\n  - password\n  note: 'Derived from the provider''s live OpenID Connect discovery document, not from\n    an OpenAPI securitySchemes block — Ambience publishes no public OpenAPI. The Integration\n    API itself is described only as \"secure authentication and access control\"; credentials\n    are issued on request.'\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.ambiencehealthcare.com/.well-known/openid-configuration\n  issuer: https://auth.ambiencehealthcare.com/\n  sources:\n  - well-known/ambience-healthcare-openid-configuration.json\n  endpoints:\n\
  \    authorization: https://auth.ambiencehealthcare.com/authorize\n    token: https://auth.ambiencehealthcare.com/oauth/token\n    device_authorization: https://auth.ambiencehealthcare.com/oauth/device/code\n    userinfo: https://auth.ambiencehealthcare.com/userinfo\n    jwks: https://auth.ambiencehealthcare.com/.well-known/jwks.json\n    registration: https://auth.ambiencehealthcare.com/oidc/register\n    revocation: https://auth.ambiencehealthcare.com/oauth/revoke\n    backchannel_authentication: https://auth.ambiencehealthcare.com/bc-authorize\n    mfa_challenge: https://auth.ambiencehealthcare.com/mfa/challenge\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/ambience-healthcare-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.ambiencehealthcare.com/authorize\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\n  - flow:\
  \ deviceCode\n    deviceAuthorizationUrl: https://auth.ambiencehealthcare.com/oauth/device/code\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.ambiencehealthcare.com/authorize\n    note: advertised in response_types_supported; not recommended, recorded as observed\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\nclient_authentication:\n  methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  signing_algs:\n\
  \  - RS256\n  - RS384\n  - PS256\nhardening:\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  dpop_signing_algs:\n  - ES256\n  mfa: true\n  backchannel_logout: true\n  dynamic_client_registration: true\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  observations:\n  - HS256 is advertised for ID token signing alongside RS256/PS256 — a symmetric option\n    that FAPI-grade profiles disallow.\n  - The `implicit` response types and the `password` grant remain enabled on the tenant.\n  - PKCE advertises `plain` in addition to `S256`.\ndownstream_auth:\n  note: 'Ambience authenticates OUTBOUND into customer EHRs as a client. Per the provider''s\n    informatics page it uses SMART on FHIR for Epic (deployed via the Epic Toolbox\n    inside Hyperspace and Haiku), the athenahealth Marketplace / MDP programme for\n    athenahealth, and FHIR plus REST APIs for Oracle Cerner Millennium.'\n  source: https://www.ambiencehealthcare.com/informatics\nx-evidence:\n  fetched:\
  \ '2026-07-31'\n  url: https://auth.ambiencehealthcare.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambience-healthcare/refs/heads/main/authentication/ambience-healthcare-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Documentation
- Ambient AI
- Medical Coding
- Electronic Health Records
- FHIR
- Health IT
- Speech Recognition
---
