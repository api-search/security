---
api_key_in:
- header
- query
api_specs:
- filename: krisp-developers-openapi.yml
  format: yaml
  label: Krisp Voice Translation API
  slug: voice-translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/openapi/krisp-developers-openapi.yml
- filename: krisp-developers-openapi.yml
  format: yaml
  label: Krisp SDK & Model Downloads API
  slug: sdk-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/openapi/krisp-developers-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Krisp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Krisp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Krisp
provider_slug: krisp
scheme_count: 2
schemes:
- applies_to:
  - GET /v2/sdk/voice-translation/session/token
  - GET /voice-translation/languages
  - GET /v2/sdk/versions/{id}/download-urls
  in: header
  issued_at: https://developers.krisp.ai/
  name: ApiKeyAuth
  note: The docs render this header two ways — 'api-key API_KEY' in the session-token example and 'API-Key {api-key}' on the list-languages endpoint. Recorded verbatim; the scheme value appears to be case-insensitive.
  parameter: Authorization
  scope: REST — api.developers.krisp.ai
  sources:
  - https://sdk-docs.krisp.ai/docs/voice-translation-api.md
  - https://sdk-docs.krisp.ai/docs/programmatic-sdk-model-downloads-api.md
  type: apiKey
  value_format: api-key {API_KEY}
- in: query
  name: SessionKeyAuth
  note: Passed as a query parameter on the WebSocket URL because browsers cannot set headers on WSS handshakes.
  parameter: authorization
  scope: streaming — wss://streaming.krisp.ai/vt
  sources:
  - https://sdk-docs.krisp.ai/docs/voice-translation-api.md
  type: apiKey
  value_format: Api-Key {SESSION_KEY}
slug: krisp-authentication
source_filename: krisp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://sdk-docs.krisp.ai/docs/voice-translation-api.md\ndocs: https://sdk-docs.krisp.ai/docs/voice-translation-api.md\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  note: >-\n    Krisp uses a two-stage API-key model. A long-lived account API key (issued in the developer dashboard\n    at https://developers.krisp.ai/) authenticates REST calls via an Authorization header. That key mints\n    a short-lived session key which is the only credential passed to the streaming WebSocket endpoint, so\n    the account key never reaches the browser. There is no OAuth 2.0, OpenID Connect, or mutual TLS\n    surface; /.well-known/oauth-authorization-server and a valid /.well-known/openid-configuration are\n    both absent.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'api-key {API_KEY}'\n  scope: REST — api.developers.krisp.ai\n  issued_at: https://developers.krisp.ai/\n\
  \  applies_to:\n  - GET /v2/sdk/voice-translation/session/token\n  - GET /voice-translation/languages\n  - GET /v2/sdk/versions/{id}/download-urls\n  sources: [https://sdk-docs.krisp.ai/docs/voice-translation-api.md, https://sdk-docs.krisp.ai/docs/programmatic-sdk-model-downloads-api.md]\n  note: >-\n    The docs render this header two ways — 'api-key API_KEY' in the session-token example and\n    'API-Key {api-key}' on the list-languages endpoint. Recorded verbatim; the scheme value appears to be\n    case-insensitive.\n- name: SessionKeyAuth\n  type: apiKey\n  in: query\n  parameter: authorization\n  value_format: 'Api-Key {SESSION_KEY}'\n  scope: streaming — wss://streaming.krisp.ai/vt\n  sources: [https://sdk-docs.krisp.ai/docs/voice-translation-api.md]\n  note: Passed as a query parameter on the WebSocket URL because browsers cannot set headers on WSS handshakes.\nsession_keys:\n  mint_operation: GET https://api.developers.krisp.ai/v2/sdk/voice-translation/session/token\n  parameter:\
  \ expiration_ttl\n  parameter_units: minutes\n  ttl_min: 5\n  ttl_max: 1440\n  response_fields: [session_key, expires_at, key_id, status, type]\n  recommended_pattern: >-\n    Mint the session key on your backend with the account API key, then hand only the session key to the\n    client that opens the WebSocket.\nauth_failure:\n  code: 401\n  reason: Unauthorized\n  causes: [missing API key, invalid API key, expired API key]\n  source: errors/krisp-error-codes.yml\nrelated:\n- conventions/krisp-conventions.yml\n- errors/krisp-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/authentication/krisp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai
- Voice AI
- Speech
- Audio
- Noise Cancellation
- Speech Translation
- Real Time Communications
- WebRTC
- Conversational AI
- SDK
- Machine Learning
---
