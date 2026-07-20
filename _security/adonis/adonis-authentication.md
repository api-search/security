---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Adonis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- tokenExchange
overview: Adonis secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, and tokenExchange flow(s).
provider_name: Adonis
provider_slug: adonis
scheme_count: 2
schemes:
- issuer: https://auth.adonis.io/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.adonis.io/.well-known/openid-configuration
  sources:
  - well-known/adonis-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://auth.adonis.io/authorize
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  jwksUrl: https://auth.adonis.io/.well-known/jwks.json
  name: OAuth2
  revocationUrl: https://auth.adonis.io/oauth/revoke
  sources:
  - well-known/adonis-oauth-authorization-server.json
  tokenUrl: https://auth.adonis.io/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
  userinfoUrl: https://auth.adonis.io/userinfo
slug: adonis-authentication
source_filename: adonis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.adonis.io/.well-known/openid-configuration\ndocs: https://adonis.io/platform\nsummary:\n  types: [oauth2, openIdConnect]\n  identity_provider: Auth0\n  issuer: https://auth.adonis.io/\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode, tokenExchange]\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.adonis.io/.well-known/openid-configuration\n  issuer: https://auth.adonis.io/\n  sources: [well-known/adonis-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  authorizationUrl: https://auth.adonis.io/authorize\n  tokenUrl: https://auth.adonis.io/oauth/token\n  userinfoUrl: https://auth.adonis.io/userinfo\n  jwksUrl: https://auth.adonis.io/.well-known/jwks.json\n  revocationUrl: https://auth.adonis.io/oauth/revoke\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  sources: [well-known/adonis-oauth-authorization-server.json]\nnotes: >-\n  Auth is provided by Auth0 (issuer https://auth.adonis.io/). client_credentials\n  supports machine-to-machine partner/API integrations; authorization_code (with\n  PKCE via the \"none\" auth method for public clients) backs the app.adonis.io\n  web application. Scopes are documented in scopes/adonis-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adonis/refs/heads/main/authentication/adonis-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthcare
- Revenue Cycle Management
- RCM
- Medical Billing
- Health IT
- Eligibility Verification
- Claims
- Payments
- Artificial Intelligence
- Automation
---
