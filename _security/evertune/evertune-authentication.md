---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Evertune Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
- jwtBearer
- password
overview: Evertune secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, refreshToken, tokenExchange, jwtBearer, and password flow(s).
provider_name: Evertune
provider_slug: evertune
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://auth.evertune.ai/authorize
    backchannel_authentication: https://auth.evertune.ai/bc-authorize
    device_authorization: https://auth.evertune.ai/oauth/device/code
    end_session: https://auth.evertune.ai/oidc/logout
    jwks: https://auth.evertune.ai/.well-known/jwks.json
    mfa_challenge: https://auth.evertune.ai/mfa/challenge
    registration: https://auth.evertune.ai/oidc/register
    revocation: https://auth.evertune.ai/oauth/revoke
    token: https://auth.evertune.ai/oauth/token
    userinfo: https://auth.evertune.ai/userinfo
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.evertune.ai/
  mfa: true
  name: Auth0OIDC
  openIdConnectUrl: https://auth.evertune.ai/.well-known/openid-configuration
  provider: Auth0 (custom domain on evertune.ai)
  sources:
  - well-known/evertune-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: evertune-authentication
source_filename: evertune-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.evertune.ai/.well-known/openid-configuration\nscope_of_this_artifact: >-\n  This profile describes the identity surface Evertune actually publishes: the\n  Auth0 tenant it runs on its own domain (auth.evertune.ai) to sign users in to\n  the Evertune web application at app.evertune.ai. Evertune publishes NO\n  first-party developer API, so this is NOT an API authorization contract --\n  there is no documented developer client registration, no API audience, no\n  documented API scopes, and no published token-issuance guidance for\n  third-party integrators. It is recorded because the discovery document is\n  real, anonymous, machine-readable, and served by Evertune.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  - tokenExchange\n  - jwtBearer\n  - password\nschemes:\n- name: Auth0OIDC\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://auth.evertune.ai/.well-known/openid-configuration\n  issuer: https://auth.evertune.ai/\n  provider: Auth0 (custom domain on evertune.ai)\n  sources:\n  - well-known/evertune-openid-configuration.json\n  endpoints:\n    authorization: https://auth.evertune.ai/authorize\n    token: https://auth.evertune.ai/oauth/token\n    userinfo: https://auth.evertune.ai/userinfo\n    jwks: https://auth.evertune.ai/.well-known/jwks.json\n    registration: https://auth.evertune.ai/oidc/register\n    revocation: https://auth.evertune.ai/oauth/revoke\n    device_authorization: https://auth.evertune.ai/oauth/device/code\n    end_session: https://auth.evertune.ai/oidc/logout\n    backchannel_authentication: https://auth.evertune.ai/bc-authorize\n    mfa_challenge: https://auth.evertune.ai/mfa/challenge\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_alg_values_supported:\n  - ES256\n  mfa: true\nx-evidence:\n- url: https://auth.evertune.ai/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-13'\n- url: https://auth.evertune.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-13'\n- url: https://auth.evertune.ai/.well-known/jwks.json\n\
  \  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evertune/refs/heads/main/authentication/evertune-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Generative Engine Optimization
- AI Search
- Brand Monitoring
- Marketing Intelligence
- AI Visibility
- Analytics
- Artificial Intelligence
---
