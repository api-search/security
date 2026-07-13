---
api_key_in:
- cookie
- header
api_specs:
- filename: axway-amplify-platform-openapi-original.json
  format: json
  label: Axway Amplify Platform API
  slug: axway-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-amplify-platform-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Axway Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Axway secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Axway
provider_slug: axway
scheme_count: 6
schemes:
- description: Auth token for internal services
  in: header
  name: AuthToken
  parameter: x-auth-token
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: apiKey
- bearerFormat: jwt
  description: Service account access token
  name: BearerClient
  scheme: bearer
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: http
- description: Multi-factor authentication code
  in: header
  name: MFA
  parameter: x-auth-code
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: implicit
    scopes: 0
  name: OAuth2
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: oauth2
- description: User password
  in: header
  name: Password
  parameter: x-auth-password
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: apiKey
- description: Platform session cookie
  in: cookie
  name: SessionCookie
  parameter: connect.sid
  sources:
  - openapi/axway-amplify-platform-openapi-original.json
  type: apiKey
slug: axway-authentication
source_filename: axway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/axway-amplify-platform-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: x-auth-token\n  description: Auth token for internal services\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n- name: BearerClient\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  description: Service account access token\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n- name: MFA\n  type: apiKey\n  in: header\n  parameter: x-auth-code\n  description: Multi-factor authentication code\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token\n\
  \    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token\n    scopes: 0\n  - flow: implicit\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n    scopes: 0\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n- name: Password\n  type: apiKey\n  in: header\n  parameter: x-auth-password\n  description: User password\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: connect.sid\n  description: Platform session cookie\n  sources:\n  - openapi/axway-amplify-platform-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/authentication/axway-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- API Management
- Enterprise
- Integration
- Security
---
