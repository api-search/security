---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Recuro Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- tokenExchange
- jwtBearer
overview: Recuro Health secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, tokenExchange, and jwtBearer flow(s).
provider_name: Recuro Health
provider_slug: recuro-health
scheme_count: 2
schemes:
- issuer: https://auth.recurohealth.com/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.recurohealth.com/.well-known/openid-configuration
  provider: Auth0
  sources:
  - well-known/recuro-health-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.recurohealth.com/authorize
    flow: authorizationCode
    refreshUrl: https://auth.recurohealth.com/oauth/token
    tokenUrl: https://auth.recurohealth.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.recurohealth.com/oauth/token
  - authorizationUrl: https://auth.recurohealth.com/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://auth.recurohealth.com/oauth/token
  - deviceAuthorizationUrl: https://auth.recurohealth.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.recurohealth.com/oauth/token
  name: OAuth2
  sources:
  - well-known/recuro-health-oauth-authorization-server.json
  type: oauth2
slug: recuro-health-authentication
source_filename: recuro-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://auth.recurohealth.com/.well-known/openid-configuration\ndocs: https://auth.recurohealth.com/.well-known/openid-configuration\nnotes: >-\n  Derived verbatim from Recuro Health's own published OpenID Connect discovery document\n  and RFC 8414 authorization-server metadata. Recuro Health publishes no OpenAPI, so\n  there are no securitySchemes to aggregate; this profile describes the identity surface\n  that fronts the platform. The protected resource APIs behind this authorization server\n  are not publicly documented.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - deviceCode\n  - tokenExchange\n  - jwtBearer\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.recurohealth.com/.well-known/openid-configuration\n  issuer: https://auth.recurohealth.com/\n  provider: Auth0\n\
  \  sources:\n  - well-known/recuro-health-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/recuro-health-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.recurohealth.com/authorize\n    tokenUrl: https://auth.recurohealth.com/oauth/token\n    refreshUrl: https://auth.recurohealth.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.recurohealth.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.recurohealth.com/authorize\n  - flow: password\n    tokenUrl: https://auth.recurohealth.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.recurohealth.com/oauth/device/code\n    tokenUrl: https://auth.recurohealth.com/oauth/token\nendpoints:\n  issuer: https://auth.recurohealth.com/\n  authorization_endpoint: https://auth.recurohealth.com/authorize\n  token_endpoint: https://auth.recurohealth.com/oauth/token\n  userinfo_endpoint: https://auth.recurohealth.com/userinfo\n\
  \  device_authorization_endpoint: https://auth.recurohealth.com/oauth/device/code\n  jwks_uri: https://auth.recurohealth.com/.well-known/jwks.json\n  registration_endpoint: https://auth.recurohealth.com/oidc/register\n  revocation_endpoint: https://auth.recurohealth.com/oauth/revoke\n  mfa_challenge_endpoint: https://auth.recurohealth.com/mfa/challenge\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\npkce:\n  supported: true\n\
  \  code_challenge_methods:\n  - S256\n  - plain\ntokens:\n  format: JWT\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  presentation: 'Authorization: Bearer <access_token>'\n  jwks: well-known/recuro-health-jwks.json\nmfa:\n  supported: true\n  evidence: mfa_challenge_endpoint and Auth0 mfa-oob/mfa-otp/mfa-recovery-code grant types\nlogout:\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\ndynamic_client_registration:\n  supported: true\n  endpoint: https://auth.recurohealth.com/oidc/register\n  spec: RFC 7591\n  note: >-\n    Advertised in the discovery document. Not exercised by this pipeline — registration\n    is a write operation and was not attempted.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://auth.recurohealth.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recuro-health/refs/heads/main/authentication/recuro-health-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Health
- Healthcare
- Telehealth
- Virtual Care
- Digital Health
- Behavioral Health
- Primary Care
- Employee Benefits
- Health Plans
- Identity
- OpenID Connect
---
