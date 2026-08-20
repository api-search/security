---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Arundo Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- refreshToken
overview: Arundo Analytics secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, and refreshToken flow(s).
provider_name: Arundo Analytics
provider_slug: arundo-analytics
scheme_count: 2
schemes:
- issuer: https://arundo.eu.auth0.com/
  name: OpenIDConnect
  openIdConnectUrl: https://arundo.eu.auth0.com/.well-known/openid-configuration
  provider: Auth0 (EU region tenant)
  sources:
  - well-known/arundo-analytics-openid-configuration.json
  type: openIdConnect
- code_challenge_methods:
  - S256
  - plain
  dpop_signing_algs:
  - ES256
  dynamic_client_registration: true
  endpoints:
    authorization: https://arundo.eu.auth0.com/authorize
    backchannel_authentication: https://arundo.eu.auth0.com/bc-authorize
    device_authorization: https://arundo.eu.auth0.com/oauth/device/code
    jwks: https://arundo.eu.auth0.com/.well-known/jwks.json
    mfa_challenge: https://arundo.eu.auth0.com/mfa/challenge
    registration: https://arundo.eu.auth0.com/oidc/register
    revocation: https://arundo.eu.auth0.com/oauth/revoke
    token: https://arundo.eu.auth0.com/oauth/token
    userinfo: https://arundo.eu.auth0.com/userinfo
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
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  name: OAuth2
  sources:
  - well-known/arundo-analytics-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
slug: arundo-analytics-authentication
source_filename: arundo-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://arundo.eu.auth0.com/.well-known/openid-configuration\nnote: >-\n  Arundo publishes no OpenAPI, so there are no securitySchemes to derive from. This\n  profile is probed directly from the OpenID Connect discovery document served by the\n  Auth0 EU tenant that fronts Arundo's customer applications — carbonpath.arundo.com\n  redirects to https://arundo.eu.auth0.com/u/login. It describes how Arundo\n  authenticates users and machine clients; it is NOT a description of a public\n  Arundo API, because Arundo does not document one.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - deviceCode\n  - refreshToken\n  api_key_in: []\n  mfa: true\n  pkce: true\n  dpop: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://arundo.eu.auth0.com/.well-known/openid-configuration\n  issuer: https://arundo.eu.auth0.com/\n\
  \  provider: Auth0 (EU region tenant)\n  sources:\n  - well-known/arundo-analytics-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/arundo-analytics-oauth-authorization-server.json\n  endpoints:\n    authorization: https://arundo.eu.auth0.com/authorize\n    token: https://arundo.eu.auth0.com/oauth/token\n    userinfo: https://arundo.eu.auth0.com/userinfo\n    revocation: https://arundo.eu.auth0.com/oauth/revoke\n    device_authorization: https://arundo.eu.auth0.com/oauth/device/code\n    backchannel_authentication: https://arundo.eu.auth0.com/bc-authorize\n    registration: https://arundo.eu.auth0.com/oidc/register\n    jwks: https://arundo.eu.auth0.com/.well-known/jwks.json\n    mfa_challenge: https://arundo.eu.auth0.com/mfa/challenge\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n \
  \ - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  code_challenge_methods:\n  - S256\n  - plain\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\n  dynamic_client_registration: true\ngaps:\n- No public developer authentication documentation — Arundo publishes no developer\n  portal, no API reference and no getting-started page for the Foundation APIs.\n- Machine-to-machine access (client_credentials) is advertised by the tenant metadata,\n  but the audience/API identifiers, the scope vocabulary and the credential-issuance\n  process are not published anywhere public.\nx-evidence:\n\
  \  fetched: '2026-08-06'\n  url: https://arundo.eu.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arundo-analytics/refs/heads/main/authentication/arundo-analytics-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Industrial AI
- Industrial IoT
- Analytics
- Machine-Learning
- Time Series
- Asset Performance Management
- Anomaly Detection
- Energy
- Maritime
- Oil and Gas
- Manufacturing
---
