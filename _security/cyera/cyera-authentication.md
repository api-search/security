---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: 'Cyera authenticates API clients with OAuth 2.0 / OpenID Connect against its authorization server at auth.cyera.io. Programmatic/API access uses the client_credentials grant: a Client ID + Client Secret (generated in the Cyera console) are exchanged at the token endpoint for a short-lived JWT bearer token that is then sent as `Authorization: Bearer <jwt>` to the API host (api.cyera.io, or the regional api-eu.cyera.io). Integration vendors also document a `/v1/login` convenience endpoint that takes the Client ID + Client Secret and returns the same short-lived JWT. Interactive console/user login uses the authorization_code flow with PKCE (S256).'
kind: authentication
layout: security
method: searched
name: Cyera Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- tokenExchange
overview: Cyera secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, and tokenExchange flow(s).
provider_name: Cyera
provider_slug: cyera
scheme_count: 3
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  scopes:
  - openid
  - profile
  - email
  source: https://auth.cyera.io/.well-known/openid-configuration
  tokenUrl: https://auth.cyera.io/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- authorizationUrl: https://auth.cyera.io/oauth/authorize
  flow: authorizationCode
  name: oauth2AuthorizationCode
  pkce: S256
  scopes:
  - openid
  - profile
  - email
  source: https://auth.cyera.io/.well-known/openid-configuration
  tokenUrl: https://auth.cyera.io/oauth/token
  type: oauth2
- bearerFormat: JWT
  description: Short-lived JWT sent as Authorization Bearer to api.cyera.io.
  name: bearerAuth
  scheme: bearer
  source: vendor integration docs (Atlan, Axonius, Swimlane, BlinkOps)
  type: http
slug: cyera-authentication
source_filename: cyera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.cyera.io/.well-known/openid-configuration\ndocs: https://support.cyera.io/hc/en-us\nsummary:\n  types: [oauth2, openIdConnect, http]\n  http_scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials, authorizationCode, deviceCode, tokenExchange]\n  api_key_in: []\ndescription: >-\n  Cyera authenticates API clients with OAuth 2.0 / OpenID Connect against its\n  authorization server at auth.cyera.io. Programmatic/API access uses the\n  client_credentials grant: a Client ID + Client Secret (generated in the Cyera\n  console) are exchanged at the token endpoint for a short-lived JWT bearer\n  token that is then sent as `Authorization: Bearer <jwt>` to the API host\n  (api.cyera.io, or the regional api-eu.cyera.io). Integration vendors also\n  document a `/v1/login` convenience endpoint that takes the Client ID + Client\n  Secret and returns the same short-lived JWT. Interactive console/user login\n \
  \ uses the authorization_code flow with PKCE (S256).\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.cyera.io/oauth/token\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  scopes: [openid, profile, email]\n  source: https://auth.cyera.io/.well-known/openid-configuration\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://auth.cyera.io/oauth/authorize\n  tokenUrl: https://auth.cyera.io/oauth/token\n  pkce: S256\n  scopes: [openid, profile, email]\n  source: https://auth.cyera.io/.well-known/openid-configuration\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived JWT sent as Authorization Bearer to api.cyera.io.\n  source: vendor integration docs (Atlan, Axonius, Swimlane, BlinkOps)\nendpoints:\n  issuer: https://auth.cyera.io\n  authorization_endpoint: https://auth.cyera.io/oauth/authorize\n  token_endpoint:\
  \ https://auth.cyera.io/oauth/token\n  userinfo_endpoint: https://auth.cyera.io/identity/resources/users/v2/me\n  jwks_uri: https://auth.cyera.io/.well-known/jwks.json\n  device_authorization_endpoint: https://auth.cyera.io/oauth/device/authorize\n  end_session_endpoint: https://auth.cyera.io/oauth/logout\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:device_code\n  id_token_signing_alg_values_supported: [RS256, ES256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyera/refs/heads/main/authentication/cyera-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Company
- Cybersecurity
- Data Security
- DSPM
- Data Security Posture Management
- Data Classification
- Cloud Security
- Compliance
- MCP
- AI Security
---
