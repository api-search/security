---
api_key_in:
- cookie
api_specs:
- filename: ninjaone-openapi-original.yml
  format: yaml
  label: NinjaOne Public API 2.0
  slug: ninjaone-public-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/openapi/ninjaone-openapi-original.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ninjaone Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: NinjaOne secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: NinjaOne
provider_slug: ninjaone
scheme_count: 2
schemes:
- bearerFormat: bearer
  name: oauth2
  scheme: bearer
  sources:
  - openapi/ninjaone-openapi-original.yml
  type: http
- in: cookie
  name: sessionKey
  parameter: sessionKey
  sources:
  - openapi/ninjaone-openapi-original.yml
  type: apiKey
slug: ninjaone-authentication
source_filename: ninjaone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ninjaone-openapi-original.yml\ndocs: https://www.ninjaone.com/docs/application-programming-interface-api/oauth-token-configuration/\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - refreshToken\nnotes: >-\n  The NinjaOne Public API is secured with OAuth 2.0. Machine-to-machine\n  integrations use the client-credentials grant; interactive apps use the\n  authorization-code grant (PKCE, S256) with refresh tokens. Tokens are Bearer\n  tokens sent in the Authorization header and expire in 3600 seconds. The\n  OpenAPI models the bearer requirement as an http/bearer scheme named \"oauth2\";\n  the OAuth 2.0 endpoints below are published in the authorization-server\n  metadata at https://app.ninjarmm.com/.well-known/oauth-authorization-server.\noauth2:\n  authorization_endpoint: https://app.ninjarmm.com/ws/oauth/authorize\n  token_endpoint:\
  \ https://app.ninjarmm.com/ws/oauth/token\n  revocation_endpoint: https://app.ninjarmm.com/ws/oauth/revoke\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  code_challenge_methods_supported:\n  - S256\n  scopes:\n  - monitoring\n  - management\n  - control\nschemes:\n- name: oauth2\n  type: http\n  scheme: bearer\n  bearerFormat: bearer\n  sources:\n  - openapi/ninjaone-openapi-original.yml\n- name: sessionKey\n  type: apiKey\n  in: cookie\n  parameter: sessionKey\n  sources:\n  - openapi/ninjaone-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/authentication/ninjaone-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Developer Tools
- IT Management
- RMM
- Endpoint Management
- MSP
- IT Operations
- Monitoring
- Automation
- Ticketing
---
