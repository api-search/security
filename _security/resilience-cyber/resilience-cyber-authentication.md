---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Resilience Cyber Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
overview: Resilience secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, and tokenExchange flow(s).
provider_name: Resilience
provider_slug: resilience-cyber
scheme_count: 2
schemes:
- issuer: https://auth.cyberresilience.com/
  name: Auth0OIDC
  openIdConnectUrl: https://auth.cyberresilience.com/.well-known/openid-configuration
  sources:
  - well-known/resilience-cyber-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.cyberresilience.com/authorize
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    pkce: required-in-practice
    refreshUrl: https://auth.cyberresilience.com/oauth/token
    tokenUrl: https://auth.cyberresilience.com/oauth/token
  - flow: clientCredentials
    note: Advertised in tenant metadata. No partner client-credentials onboarding is documented publicly anywhere on cyberresilience.com.
    tokenUrl: https://auth.cyberresilience.com/oauth/token
  - deviceAuthorizationUrl: https://auth.cyberresilience.com/oauth/device/code
    flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
  name: Auth0OAuth2
  sources:
  - well-known/resilience-cyber-oauth-authorization-server.json
  type: oauth2
slug: resilience-cyber-authentication
source_filename: resilience-cyber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cyberresilience.com/.well-known/openid-configuration\ndocs: https://auth.cyberresilience.com/.well-known/openid-configuration\nlocal_copy: well-known/resilience-cyber-openid-configuration.json\nnote: >-\n  Resilience publishes no OpenAPI, so this profile is not derived from a spec —\n  it is read verbatim from the Auth0 tenant metadata that guards\n  portal.cyberresilience.com, plus the live /authorize redirect the portal\n  issues. This is the only publicly documented machine-readable surface on the\n  estate. Anyone integrating still needs an appointed-broker relationship and a\n  client_id issued by Resilience; there is no self-serve registration.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  - tokenExchange\n  bearer_format: JWT\n  self_serve_signup: false\n  audience_gated: true\nschemes:\n\
  - name: Auth0OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.cyberresilience.com/.well-known/openid-configuration\n  issuer: https://auth.cyberresilience.com/\n  sources:\n  - well-known/resilience-cyber-openid-configuration.json\n- name: Auth0OAuth2\n  type: oauth2\n  sources:\n  - well-known/resilience-cyber-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cyberresilience.com/authorize\n    tokenUrl: https://auth.cyberresilience.com/oauth/token\n    refreshUrl: https://auth.cyberresilience.com/oauth/token\n    pkce: required-in-practice\n    code_challenge_methods:\n    - S256\n    - plain\n  - flow: clientCredentials\n    tokenUrl: https://auth.cyberresilience.com/oauth/token\n    note: >-\n      Advertised in tenant metadata. No partner client-credentials onboarding is\n      documented publicly anywhere on cyberresilience.com.\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.cyberresilience.com/oauth/device/code\n\
  \    grant: urn:ietf:params:oauth:grant-type:device_code\nendpoints:\n  issuer: https://auth.cyberresilience.com/\n  authorization: https://auth.cyberresilience.com/authorize\n  token: https://auth.cyberresilience.com/oauth/token\n  userinfo: https://auth.cyberresilience.com/userinfo\n  jwks: https://auth.cyberresilience.com/.well-known/jwks.json\n  registration: https://auth.cyberresilience.com/oidc/register\n  revocation: https://auth.cyberresilience.com/oauth/revoke\n  device_authorization: https://auth.cyberresilience.com/oauth/device/code\n  backchannel_authentication: https://auth.cyberresilience.com/bc-authorize\n  mfa_challenge: https://auth.cyberresilience.com/mfa/challenge\n  global_token_revocation: https://auth.cyberresilience.com/oauth/global-token-revocation/connection/{connectionName}\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n\
  - urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\nsender_constraining:\n  dpop: true\n  dpop_signing_alg_values_supported:\n  - ES256\n  mutual_tls: false\n  note: >-\n    DPoP (RFC 9449) proof-of-possession is advertised by the tenant; whether the\n    private product API enforces it cannot be observed anonymously.\nobserved_client:\n  source: >-\n    live 302 chain https://portal.cyberresilience.com/ ->\n    /v2/api/auth/login -> https://auth.cyberresilience.com/authorize (probed\n    2026-07-25)\n  response_type: code\n  code_challenge_method: S256\n  scope: openid\
  \ profile email offline_access\n  audience: https://api.prod.resilienceinsurance.app\n  redirect_uri: https://portal.cyberresilience.com/v2/api/auth/callback\n  prompt: login\n  note: client_id is deliberately not recorded here.\nresource_server:\n  audience: https://api.prod.resilienceinsurance.app\n  published: false\n  oauth_protected_resource_metadata: false\n  note: >-\n    The private product API exists and is named as an OAuth audience, but it\n    returns 404 anonymously for /, /openapi.json, /openapi.yaml, /swagger.json,\n    /v1/openapi.json, /api-docs, /docs, /redoc, /graphql and /mcp, and serves no\n    RFC 9728 protected-resource metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilience-cyber/refs/heads/main/authentication/resilience-cyber-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- United States
- Cyber Insurance
- Property and Casualty
- Insurtech
- Underwriting
- Claims
- Risk Data
- Technology Errors and Omissions
- Broker
- Specialty Insurance
---
