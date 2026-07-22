---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Eliseai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- implicit
overview: EliseAI secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, and implicit flow(s).
provider_name: EliseAI
provider_slug: eliseai
scheme_count: 2
schemes:
- issuer: https://login.meetelise.com/
  name: OpenIDConnect
  openIdConnectUrl: https://login.meetelise.com/.well-known/openid-configuration
  sources:
  - well-known/eliseai-openid-configuration.json
  type: openIdConnect
- code_challenge_methods:
  - S256
  - plain
  endpoints:
    authorization: https://login.meetelise.com/authorize
    device_authorization: https://login.meetelise.com/oauth/device/code
    jwks: https://login.meetelise.com/.well-known/jwks.json
    registration: https://login.meetelise.com/oidc/register
    revocation: https://login.meetelise.com/oauth/revoke
    token: https://login.meetelise.com/oauth/token
    userinfo: https://login.meetelise.com/userinfo
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://login.meetelise.com/
  name: OAuth2
  sources:
  - well-known/eliseai-oauth-authorization-server.json
  type: oauth2
slug: eliseai-authentication
source_filename: eliseai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://login.meetelise.com/.well-known/openid-configuration\ndocs: https://login.meetelise.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  identity_provider: Auth0\n  issuer: https://login.meetelise.com/\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken, implicit]\n  token_endpoint_auth: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  pkce: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.meetelise.com/.well-known/openid-configuration\n  issuer: https://login.meetelise.com/\n  sources: [well-known/eliseai-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  issuer: https://login.meetelise.com/\n  endpoints:\n    authorization: https://login.meetelise.com/authorize\n    token: https://login.meetelise.com/oauth/token\n    device_authorization: https://login.meetelise.com/oauth/device/code\n\
  \    userinfo: https://login.meetelise.com/userinfo\n    revocation: https://login.meetelise.com/oauth/revoke\n    registration: https://login.meetelise.com/oidc/register\n    jwks: https://login.meetelise.com/.well-known/jwks.json\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  code_challenge_methods: [S256, plain]\n  sources: [well-known/eliseai-oauth-authorization-server.json]\nnotes: >-\n  Derived from EliseAI's live Auth0 OIDC/OAuth 2.0 discovery documents at\n  login.meetelise.com. This is the platform (app.meetelise.com) identity surface;\n  EliseAI does not publish a self-serve public API with an OpenAPI spec — partner\n  API/integration access is provisioned through the EliseAI developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliseai/refs/heads/main/authentication/eliseai-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Property Management
- Real Estate
- Healthcare
- Leasing
- Voice AI
- Automation
- CRM
---
