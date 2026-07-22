---
api_key_in:
- header
api_specs:
- filename: safello-institutional-openapi.json
  format: json
  label: Safello Institutional API
  slug: safello-institutional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-institutional-openapi.json
- filename: safello-app-openapi.json
  format: json
  label: Safello App API
  slug: safello-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-app-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Safello Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- urn:safello:params:oauth:grant-type:bankid
overview: Safello secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and urn:safello:params:oauth:grant-type:bankid flow(s).
provider_name: Safello
provider_slug: safello
scheme_count: 4
schemes:
- in: header
  name: AccessToken
  parameter: Access-Token
  sources:
  - openapi/safello-app-openapi.json
  type: apiKey
- in: header
  name: AppId
  parameter: App-Id
  sources:
  - openapi/safello-app-openapi.json
  type: apiKey
- flows:
  - flow: urn:safello:params:oauth:grant-type:bankid
    scopes: 8
    tokenUrl: /oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /oauth2/token
  - flow: authorizationCode
    scopes: 8
    tokenUrl: /oauth2/token
  name: OAuth2
  sources:
  - openapi/safello-institutional-openapi.json
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/safello-institutional-openapi.json
  type: http
slug: safello-authentication
source_filename: safello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/safello-app-openapi.json, openapi/safello-institutional-openapi.json\ndocs: https://safello.github.io/safello-api/docs/getting-started/getting-started-auth\nauthorization_server:\n  metadata: https://api.safello.com/.well-known/oauth-authorization-server\n  issuer: https://api.safello.com\n  authorization_endpoint: https://api.safello.com/oauth2/authorize\n  token_endpoint: https://api.safello.com/oauth2/token\n  jwks_uri: https://api.safello.com/oauth2/jwks\n  introspection_endpoint: https://api.safello.com/oauth2/introspect\n  revocation_endpoint: https://api.safello.com/oauth2/revoke\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt]\n  grant_types_supported: [authorization_code, client_credentials, refresh_token]\n  code_challenge_methods_supported: [S256]\n  access_token_format: JWT\n  access_token_ttl_seconds: 300\nsummary:\n  types:\n  - apiKey\n\
  \  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - urn:safello:params:oauth:grant-type:bankid\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  sources:\n  - openapi/safello-app-openapi.json\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: App-Id\n  sources:\n  - openapi/safello-app-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: urn:safello:params:oauth:grant-type:bankid\n    tokenUrl: /oauth2/token\n    scopes: 8\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n    scopes: 1\n  - flow: authorizationCode\n    tokenUrl: /oauth2/token\n    scopes: 8\n  sources:\n  - openapi/safello-institutional-openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/safello-institutional-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/authentication/safello-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Fintech
- Cryptocurrency
- Bitcoin
- Brokerage
- Payments
- Sweden
- Trading
- KYC
- BankID
---
