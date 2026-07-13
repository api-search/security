---
api_key_in:
- header
- query
api_specs:
- filename: sse
  format: yaml
  label: Neuphonic TTS SSE API
  slug: neuphonic-tts-sse-api
  spec_type: OpenAPI
  url: https://docs.neuphonic.com/api-reference/tts/sse
- filename: websocket
  format: yaml
  label: Neuphonic TTS WebSocket API
  slug: neuphonic-tts-websocket-api
  spec_type: AsyncAPI
  url: https://docs.neuphonic.com/api-reference/tts/websocket
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Neuphonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neuphonic secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neuphonic
provider_slug: neuphonic
scheme_count: 2
schemes:
- description: API key passed via the X-API-KEY request header.
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/neuphonic-openapi.yml
  type: apiKey
- description: API key passed as a query parameter (used for WebSocket connections).
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/neuphonic-openapi.yml
  type: apiKey
slug: neuphonic-authentication
source_filename: neuphonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neuphonic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key passed via the X-API-KEY request header.\n  sources:\n  - openapi/neuphonic-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter (used for WebSocket connections).\n  sources:\n  - openapi/neuphonic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuphonic/refs/heads/main/authentication/neuphonic-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Text-to-Speech
- Voice AI
- Audio
- Streaming
- WebSocket
- Voice Cloning
- Conversational AI
- Real-Time
- Multilingual
- On-Device AI
---
