---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lightforce Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- password
- refreshToken
- tokenExchange
overview: Lightforce secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, password, refreshToken, and tokenExchange flow(s).
provider_name: Lightforce
provider_slug: lightforce
scheme_count: 2
schemes:
- issuer: https://id.lightforceortho.com/
  name: OpenIDConnect
  openIdConnectUrl: https://id.lightforceortho.com/.well-known/openid-configuration
  sources:
  - well-known/lightforce-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: authorizationCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://id.lightforceortho.com/oauth/token
  - deviceAuthorizationUrl: https://id.lightforceortho.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  name: OAuth2
  sources:
  - well-known/lightforce-openid-configuration.json
  type: oauth2
slug: lightforce-authentication
source_filename: lightforce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://id.lightforceortho.com/.well-known/openid-configuration\ndocs: https://id.lightforceortho.com/.well-known/openid-configuration\nnotes: >-\n  Derived verbatim from the live OpenID Connect discovery document served by the\n  LightForce identity host. There is no public OpenAPI to derive securitySchemes from,\n  so the auth profile is taken directly from OIDC discovery. Client registration is\n  gated in practice: LightForce does not publish a developer program, and the\n  authorization surface exists to authenticate orthodontic practice users into the\n  LightForce Doctor Portal.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - deviceCode\n  - password\n  - refreshToken\n  - tokenExchange\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  mfa: true\n  dpop: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://id.lightforceortho.com/.well-known/openid-configuration\n  issuer: https://id.lightforceortho.com/\n  sources:\n  - well-known/lightforce-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/lightforce-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.lightforceortho.com/authorize\n    tokenUrl: https://id.lightforceortho.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://id.lightforceortho.com/authorize\n  - flow: clientCredentials\n    tokenUrl: https://id.lightforceortho.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://id.lightforceortho.com/oauth/device/code\n    tokenUrl: https://id.lightforceortho.com/oauth/token\nendpoints:\n  authorization: https://id.lightforceortho.com/authorize\n  token: https://id.lightforceortho.com/oauth/token\n  userinfo: https://id.lightforceortho.com/userinfo\n  device_authorization: https://id.lightforceortho.com/oauth/device/code\n\
  \  backchannel_authentication: https://id.lightforceortho.com/bc-authorize\n  mfa_challenge: https://id.lightforceortho.com/mfa/challenge\n  revocation: https://id.lightforceortho.com/oauth/revoke\n  global_token_revocation: https://id.lightforceortho.com/oauth/global-token-revocation/connection/{connectionName}\n  registration: https://id.lightforceortho.com/oidc/register\n  jwks: https://id.lightforceortho.com/.well-known/jwks.json\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n\
  - none\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\ndpop_signing_alg_values_supported:\n- ES256\nbackchannel_logout_supported: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightforce/refs/heads/main/authentication/lightforce-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Healthtech
- Orthodontics
- Dentistry
- Medical Devices
- 3D Printing
- Digital Manufacturing
- Identity
---
