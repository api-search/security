---
api_key_in: []
api_specs:
- filename: doximity-oauth-openapi.yml
  format: yaml
  label: Doximity OAuth & OpenID Connect API
  slug: doximity-oauth-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doximity/refs/heads/main/openapi/doximity-oauth-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Doximity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- deviceCode
overview: Doximity secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and deviceCode flow(s).
provider_name: Doximity
provider_slug: doximity
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.doximity.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://auth.doximity.com/oauth/token
    scope_count: 21
    tokenUrl: https://auth.doximity.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  name: doximityOAuth
  notes: Authorization Code grant with mandatory PKCE (S256). Client authentication at the token endpoint uses HTTP Basic (client_secret_basic). Access tokens are bearer tokens with a typical 1800s lifetime; refresh tokens rotate access. The device_code grant supports input-constrained clients.
  sources:
  - openapi/doximity-oauth-openapi.yml
  type: oauth2
- id_token_signing_alg: RS256
  jwks_uri: https://auth.doximity.com/.well-known/jwks.json
  name: openIdConnect
  openIdConnectUrl: https://auth.doximity.com/.well-known/openid-configuration
  sources:
  - openapi/doximity-oauth-openapi.yml
  type: openIdConnect
  userinfo_endpoint: https://auth.doximity.com/oauth/userinfo
slug: doximity-authentication
source_filename: doximity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.doximity.com/developers/documentation\ndocs: https://www.doximity.com/developers/documentation\ndiscovery: https://auth.doximity.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, deviceCode]\n  pkce: required\n  pkce_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  response_types: [\"code\", \"code id_token\", \"id_token\"]\nschemes:\n- name: doximityOAuth\n  type: oauth2\n  sources: [openapi/doximity-oauth-openapi.yml]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.doximity.com/oauth/authorize\n    tokenUrl: https://auth.doximity.com/oauth/token\n    refreshUrl: https://auth.doximity.com/oauth/token\n    scope_count: 21\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  notes: >-\n    Authorization\
  \ Code grant with mandatory PKCE (S256). Client authentication at the token\n    endpoint uses HTTP Basic (client_secret_basic). Access tokens are bearer tokens with a\n    typical 1800s lifetime; refresh tokens rotate access. The device_code grant supports\n    input-constrained clients.\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.doximity.com/.well-known/openid-configuration\n  sources: [openapi/doximity-oauth-openapi.yml]\n  id_token_signing_alg: RS256\n  jwks_uri: https://auth.doximity.com/.well-known/jwks.json\n  userinfo_endpoint: https://auth.doximity.com/oauth/userinfo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doximity/refs/heads/main/authentication/doximity-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthtech
- Identity
- OAuth
- OpenID Connect
- Authentication
- Physician Network
- Healthcare
- SSO
- Verification
---
