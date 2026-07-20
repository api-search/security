---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Datum Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- jwtBearer
- refreshToken
- implicit
overview: Datum secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, jwtBearer, refreshToken, and implicit flow(s).
provider_name: Datum
provider_slug: datum
scheme_count: 2
schemes:
- name: OIDC
  openIdConnectUrl: https://www.datum.net/.well-known/openid-configuration
  sources:
  - well-known/datum-openid-configuration.json
  type: openIdConnect
- code_challenge_methods:
  - S256
  endpoints:
    authorization: https://auth.datum.net/oauth/v2/authorize
    device_authorization: https://auth.datum.net/oauth/v2/device_authorization
    end_session: https://auth.datum.net/oidc/v1/end_session
    introspection: https://auth.datum.net/oauth/v2/introspect
    jwks: https://auth.datum.net/oauth/v2/keys
    revocation: https://auth.datum.net/oauth/v2/revoke
    token: https://auth.datum.net/oauth/v2/token
    userinfo: https://auth.datum.net/oidc/v1/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - implicit
  id_token_signing_alg:
  - EdDSA
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  name: OAuth2
  sources:
  - well-known/datum-openid-configuration.json
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: oauth2
slug: datum-authentication
source_filename: datum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.datum.net/.well-known/openid-configuration\ndocs: https://www.datum.net/docs/datumctl/auth/logging-in.md\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, jwtBearer, refreshToken, implicit]\n  pkce: S256\n  api_key_in: []\n  note: >-\n    Datum Cloud authenticates with OAuth 2.0 / OIDC bearer tokens issued by\n    https://auth.datum.net. Interactive users log in via authorization-code +\n    PKCE (browser or device-code) through datumctl; CI/headless automation uses\n    service accounts (client_credentials / private_key_jwt). There are no static\n    API keys — datumctl stores tokens in the system keyring.\nissuer: https://auth.datum.net\nschemes:\n- name: OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.datum.net/.well-known/openid-configuration\n  sources: [well-known/datum-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  sources:\
  \ [well-known/datum-openid-configuration.json]\n  endpoints:\n    authorization: https://auth.datum.net/oauth/v2/authorize\n    token: https://auth.datum.net/oauth/v2/token\n    introspection: https://auth.datum.net/oauth/v2/introspect\n    userinfo: https://auth.datum.net/oidc/v1/userinfo\n    revocation: https://auth.datum.net/oauth/v2/revoke\n    device_authorization: https://auth.datum.net/oauth/v2/device_authorization\n    jwks: https://auth.datum.net/oauth/v2/keys\n    end_session: https://auth.datum.net/oidc/v1/end_session\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - implicit\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [EdDSA, RS256, RS384, RS512, ES256, ES384, ES512]\nservice_accounts:\n  supported: true\n  docs:\
  \ https://www.datum.net/docs/datumctl/auth/service-accounts.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datum/refs/heads/main/authentication/datum-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Data
- Cloud
- Networking
- Edge
- AI
- DNS
- Infrastructure
- CDN
- Developer Tools
---
