---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Lightforce Orthodontics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- refreshToken
overview: LightForce Orthodontics secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, and refreshToken flow(s).
provider_name: LightForce Orthodontics
provider_slug: lightforce-orthodontics
scheme_count: 2
schemes:
- issuer: https://id.lightforceortho.com/
  name: LightForceOIDC
  openIdConnectUrl: https://id.lightforceortho.com/.well-known/openid-configuration
  provider: Auth0
  sources:
  - well-known/lightforce-orthodontics-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: authorizationCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://id.lightforceortho.com/oauth/token
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://id.lightforceortho.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  issuer: https://id.lightforceortho.com/
  name: LightForceOAuth2
  sources:
  - well-known/lightforce-orthodontics-openid-configuration.json
  type: oauth2
slug: lightforce-orthodontics-authentication
source_filename: lightforce-orthodontics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://id.lightforceortho.com/.well-known/openid-configuration\ndocs: https://id.lightforceortho.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - deviceCode\n  - refreshToken\n  note: Derived from the provider's published OIDC discovery document. LightForce ships no\n    public OpenAPI, so no operation-level security requirements could be inspected. This\n    identity tenant fronts the LightForce Doctor Portal, not a documented public API.\nschemes:\n- name: LightForceOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://id.lightforceortho.com/.well-known/openid-configuration\n  issuer: https://id.lightforceortho.com/\n  provider: Auth0\n  sources:\n  - well-known/lightforce-orthodontics-openid-configuration.json\n- name: LightForceOAuth2\n  type: oauth2\n  issuer: https://id.lightforceortho.com/\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.lightforceortho.com/authorize\n    tokenUrl: https://id.lightforceortho.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://id.lightforceortho.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://id.lightforceortho.com/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://id.lightforceortho.com/oauth/device/code\n    tokenUrl: https://id.lightforceortho.com/oauth/token\n  sources:\n  - well-known/lightforce-orthodontics-openid-configuration.json\nendpoints:\n  authorization: https://id.lightforceortho.com/authorize\n  token: https://id.lightforceortho.com/oauth/token\n  userinfo: https://id.lightforceortho.com/userinfo\n  jwks: https://id.lightforceortho.com/.well-known/jwks.json\n  revocation: https://id.lightforceortho.com/oauth/revoke\n  registration: https://id.lightforceortho.com/oidc/register\n  device_authorization: https://id.lightforceortho.com/oauth/device/code\n\
  \  mfa_challenge: https://id.lightforceortho.com/mfa/challenge\ncapabilities:\n  pkce_methods:\n  - S256\n  - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs:\n  - RS256\n  - RS384\n  - PS256\n  response_modes:\n  - query\n  - fragment\n  - form_post\n  dynamic_client_registration: true\n  token_exchange: true\n  mfa: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightforce-orthodontics/refs/heads/main/authentication/lightforce-orthodontics-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthcare
- Orthodontics
- Medical Devices
- Dental
- 3D Printing
- Manufacturing
- Identity
---
