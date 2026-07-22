---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wiliot Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Wiliot secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Wiliot
provider_slug: wiliot
scheme_count: 3
schemes:
- description: POST the API key as the Authorization header to /v1/auth/token/api to receive a JWT access token. Obtain the API key from the Wiliot Platform account/management console.
  in: header
  method: POST
  name: ApiKeyExchange
  parameter: Authorization
  sources:
  - wiliot-api SDK security.py
  token_endpoint: https://api.wiliot.com/v1/auth/token/api
  type: apiKey
- description: POST username and password to /v1/auth/token to receive a JWT access token (used by the Management/Platform user credentials path).
  flow: password
  name: OAuth2Password
  sources:
  - wiliot-api SDK security.py
  token_endpoint: https://api.wiliot.com/v1/auth/token
  type: oauth2
- bearerFormat: JWT
  description: 'All resource calls (Platform/traceability, Edge, Manufacturing) send the exchanged access token as Authorization: Bearer <jwt>. Verified live: https://api.wiliot.com/v1/traceability/owner/{ownerId}/asset returns 401 without a valid bearer token.'
  name: BearerJWT
  scheme: bearer
  sources:
  - live probe
  type: http
slug: wiliot-authentication
source_filename: wiliot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: wiliot-api SDK (security/security.py, api_client.py) + live probe of https://api.wiliot.com/v1/\ndocs: https://developer.wiliot.com/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [password]\n  token_type: bearer-jwt\n  notes: >-\n    Wiliot uses a two-step model: a long-lived credential (API key OR OAuth\n    username/password) is exchanged for a short-lived JWT bearer access token,\n    which is then sent as Authorization on every API call. The SDK auto-refreshes\n    the token when it is within a minute of expiry.\nschemes:\n  - name: ApiKeyExchange\n    type: apiKey\n    in: header\n    parameter: Authorization\n    token_endpoint: https://api.wiliot.com/v1/auth/token/api\n    method: POST\n    description: >-\n      POST the API key as the Authorization header to /v1/auth/token/api to\n      receive a JWT access token. Obtain the API key from the Wiliot Platform\n      account/management\
  \ console.\n    sources: [wiliot-api SDK security.py]\n  - name: OAuth2Password\n    type: oauth2\n    flow: password\n    token_endpoint: https://api.wiliot.com/v1/auth/token\n    description: >-\n      POST username and password to /v1/auth/token to receive a JWT access\n      token (used by the Management/Platform user credentials path).\n    sources: [wiliot-api SDK security.py]\n  - name: BearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      All resource calls (Platform/traceability, Edge, Manufacturing) send the\n      exchanged access token as Authorization: Bearer <jwt>. Verified live:\n      https://api.wiliot.com/v1/traceability/owner/{ownerId}/asset returns 401\n      without a valid bearer token.\n    sources: [live probe]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiliot/refs/heads/main/authentication/wiliot-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Internet of Things
- Ambient IoT
- Supply Chain
- Asset Tracking
- Traceability
- Bluetooth
- Sensors
- RFID
---
