---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Black Ore Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- tokenExchange
overview: Black Ore Technologies secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and tokenExchange flow(s).
provider_name: Black Ore Technologies
provider_slug: black-ore-technologies
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  - plain
  endpoints:
    authorization: https://auth.blackore.ai/authorize
    device_authorization: https://auth.blackore.ai/oauth/device/code
    jwks_uri: https://auth.blackore.ai/.well-known/jwks.json
    mfa_challenge: https://auth.blackore.ai/mfa/challenge
    registration: https://auth.blackore.ai/oidc/register
    revocation: https://auth.blackore.ai/oauth/revoke
    token: https://auth.blackore.ai/oauth/token
    userinfo: https://auth.blackore.ai/userinfo
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://auth.blackore.ai/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.blackore.ai/.well-known/openid-configuration
  response_types:
  - code
  - token
  - id_token
  scopes_supported:
  - openid
  - profile
  - offline_access
  - email
  - phone
  - address
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: black-ore-technologies-authentication
source_filename: black-ore-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.blackore.ai/.well-known/openid-configuration\ndocs: https://blackore.ai/security\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, tokenExchange]\n  identity_provider: Auth0\n  mfa: true\n  sso: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.blackore.ai/.well-known/openid-configuration\n  issuer: https://auth.blackore.ai/\n  endpoints:\n    authorization: https://auth.blackore.ai/authorize\n    token: https://auth.blackore.ai/oauth/token\n    userinfo: https://auth.blackore.ai/userinfo\n    device_authorization: https://auth.blackore.ai/oauth/device/code\n    mfa_challenge: https://auth.blackore.ai/mfa/challenge\n    jwks_uri: https://auth.blackore.ai/.well-known/jwks.json\n    revocation: https://auth.blackore.ai/oauth/revoke\n    registration: https://auth.blackore.ai/oidc/register\n  grant_types:\n \
  \ - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  response_types: [code, token, id_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  code_challenge_methods: [S256, plain]\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - email\n  - phone\n  - address\nnotes: >-\n  Black Ore delegates identity to an Auth0 tenant. Standard OpenID Connect scopes are advertised\n  (identity/profile scopes only) — no product/resource authorization scopes are published, and\n  there is no public developer API or OpenAPI to derive resource scopes from. Enterprise SSO and\n  MFA are documented on the security page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-ore-technologies/refs/heads/main/authentication/black-ore-technologies-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Artificial Intelligence
- Financial Services
- Tax
- Accounting
- Fintech
- Automation
- Tax Preparation
---
