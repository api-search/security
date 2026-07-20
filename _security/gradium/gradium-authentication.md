---
api_key_in:
- header
api_specs:
- filename: gradium-openapi-original.json
  format: json
  label: Gradium API
  slug: gradium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradium/refs/heads/main/openapi/gradium-openapi-original.json
auth_types:
- apiKey
- bearer-token
description: ''
kind: authentication
layout: security
method: searched
name: Gradium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gradium secures its APIs with apiKey and bearer-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gradium
provider_slug: gradium
scheme_count: 2
schemes:
- applies_to: All REST endpoints and server-to-server calls.
  env_var: GRADIUM_API_KEY
  in: header
  key_prefix: gd_
  name: ApiKeyAuth
  parameter: x-api-key
  source: https://docs.gradium.ai/guides/installation
  type: apiKey
- applies_to: WebSocket endpoints (/api/speech/tts, /api/speech/asr, /api/speech/s2s)
  description: For browser/mobile WebSocket clients, exchange the server-side API key for a single-use, short-lived token via GET https://api.gradium.ai/api/api-keys/token (x-api-key header). The client connects to the WebSocket endpoint with ?token=<token>. Token is consumed on verification; issue one per connection.
  name: ShortLivedToken
  source: https://docs.gradium.ai/guides/browser-websockets
  token_endpoint: https://api.gradium.ai/api/api-keys/token
  transport: query-parameter (?token=)
  type: token-exchange
slug: gradium-authentication
source_filename: gradium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gradium.ai/guides/installation, https://docs.gradium.ai/guides/browser-websockets, https://docs.gradium.ai/guides/errors\ndocs: https://docs.gradium.ai/api-reference/introduction\nnote: >-\n  The published OpenAPI (openapi/gradium-openapi-original.json) declares no\n  components.securitySchemes; the authentication model below is captured from\n  the Gradium docs, not derived from the spec.\nsummary:\n  types: [apiKey, bearer-token]\n  api_key_in: [header]\n  api_key_header: x-api-key\n  api_key_prefix: gd_\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  key_prefix: gd_\n  env_var: GRADIUM_API_KEY\n  applies_to: All REST endpoints and server-to-server calls.\n  source: https://docs.gradium.ai/guides/installation\n- name: ShortLivedToken\n  type: token-exchange\n  description: >-\n    For browser/mobile WebSocket clients, exchange the server-side API key\
  \ for a\n    single-use, short-lived token via GET https://api.gradium.ai/api/api-keys/token\n    (x-api-key header). The client connects to the WebSocket endpoint with\n    ?token=<token>. Token is consumed on verification; issue one per connection.\n  token_endpoint: https://api.gradium.ai/api/api-keys/token\n  transport: query-parameter (?token=)\n  applies_to: WebSocket endpoints (/api/speech/tts, /api/speech/asr, /api/speech/s2s)\n  source: https://docs.gradium.ai/guides/browser-websockets\nerrors:\n  invalid_or_revoked_key:\n    code: 1008\n    rest: \"HTTP 500 plain-text body 'error from server 1008: API key is revoked or expired'\"\n    websocket: 'error message {\"type\":\"error\",\"message\":\"...\",\"code\":1008} then socket close'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradium/refs/heads/main/authentication/gradium-authentication.yml
summary_line: apiKey/bearer-token · 2 schemes
tags:
- Company
- Ai Ml
- Voice AI
- Text-to-Speech
- Speech-to-Text
- Speech-to-Speech
- Voice Cloning
- Audio
- Real-Time Streaming
- WebSocket
- Developer API
- Voice Agents
---
