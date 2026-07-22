---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Numeric Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
- clientCredentials
overview: Numeric secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, refreshToken, and clientCredentials flow(s).
provider_name: Numeric
provider_slug: numeric
scheme_count: 1
schemes:
- authorization_endpoint: https://auth.numeric.io/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  device_authorization_endpoint: https://auth.numeric.io/oauth2/device_authorization
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://auth.numeric.io/oauth2/introspection
  issuer: https://auth.numeric.io
  jwks_uri: https://auth.numeric.io/oauth2/jwks
  name: OAuth2
  registration_endpoint: https://auth.numeric.io/oauth2/register
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/numeric-openid-configuration.json
  - well-known/numeric-oauth-authorization-server.json
  token_endpoint: https://auth.numeric.io/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://auth.numeric.io/oauth2/userinfo
slug: numeric-authentication
source_filename: numeric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.numeric.io/.well-known/openid-configuration\ndocs: https://api.numeric.io/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken, clientCredentials]\n  bearer_methods: [header]\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://auth.numeric.io\n  authorization_endpoint: https://auth.numeric.io/oauth2/authorize\n  token_endpoint: https://auth.numeric.io/oauth2/token\n  device_authorization_endpoint: https://auth.numeric.io/oauth2/device_authorization\n  introspection_endpoint: https://auth.numeric.io/oauth2/introspection\n  registration_endpoint: https://auth.numeric.io/oauth2/register\n  userinfo_endpoint: https://auth.numeric.io/oauth2/userinfo\n  jwks_uri: https://auth.numeric.io/oauth2/jwks\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n\
  \  - \"urn:ietf:params:oauth:grant-type:device_code\"\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  scopes_supported: [openid, profile, email, offline_access]\n  sources:\n  - well-known/numeric-openid-configuration.json\n  - well-known/numeric-oauth-authorization-server.json\nprotected_resources:\n- resource: https://api.numeric.io/mcp\n  authorization_servers: [https://auth.numeric.io]\n  bearer_methods_supported: [header]\n  source: well-known/numeric-oauth-protected-resource-mcp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numeric/refs/heads/main/authentication/numeric-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Fintech
- Accounting
- Financial Close
- Reconciliation
- MCP
- Agent Skills
- OAuth
---
