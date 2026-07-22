---
api_key_in:
- header
api_specs:
- filename: reson8-openapi.yml
  format: yaml
  label: Reson8 Speech-to-Text API
  slug: reson8-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reson8/refs/heads/main/openapi/reson8-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Reson8 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reson8 secures its APIs with apiKey and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Reson8
provider_slug: reson8
scheme_count: 3
schemes:
- header: Authorization
  in: header
  name: ApiKey
  scenario: Direct server-to-server connections. Keys are scoped to a client, created/managed in the console. Never expose client-side.
  sources:
  - docs
  type: apiKey
  value_format: ApiKey <api_key>
- name: Bearer
  scenario: End-user / client-side connections. Short-lived access token obtained by exchanging an API key at POST /v1/auth/token (token_type Bearer, expires_in ~600s).
  scheme: bearer
  sources:
  - docs
  token_endpoint: https://api.reson8.dev/v1/auth/token
  type: http
  value_format: Bearer <access_token>
- header: Sec-WebSocket-Protocol
  name: WebSocketSubProtocol
  scenario: Browser WebSocket connections that cannot set custom headers pass the access token via the WebSocket sub-protocol.
  sources:
  - docs
  type: websocket-subprotocol
  value_format: bearer, <access_token>
slug: reson8-authentication
source_filename: reson8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.reson8.dev/documentation/general/authentication/\ndocs: https://docs.reson8.dev/documentation/general/authentication/\nsummary:\n  types: [apiKey, http-bearer]\n  api_key_in: [header]\n  api_key_header: Authorization\n  api_key_scheme_prefix: ApiKey\n  oauth2_flows: []\n  token_exchange: true\n  token_ttl_seconds: 600\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    value_format: 'ApiKey <api_key>'\n    scenario: Direct server-to-server connections. Keys are scoped to a client, created/managed in the console. Never expose client-side.\n    sources: [docs]\n  - name: Bearer\n    type: http\n    scheme: bearer\n    value_format: 'Bearer <access_token>'\n    scenario: End-user / client-side connections. Short-lived access token obtained by exchanging an API key at POST /v1/auth/token (token_type Bearer, expires_in ~600s).\n    token_endpoint: https://api.reson8.dev/v1/auth/token\n\
  \    sources: [docs]\n  - name: WebSocketSubProtocol\n    type: websocket-subprotocol\n    header: Sec-WebSocket-Protocol\n    value_format: 'bearer, <access_token>'\n    scenario: Browser WebSocket connections that cannot set custom headers pass the access token via the WebSocket sub-protocol.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reson8/refs/heads/main/authentication/reson8-authentication.yml
summary_line: apiKey/http-bearer · 3 schemes
tags:
- Speech Recognition
- Speech-to-Text
- ASR
- Voice AI
- Transcription
- Diarization
- Machine Learning
- Developers
---
