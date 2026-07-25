---
api_key_in:
- header
api_specs:
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Sonic Text-to-Speech API
  slug: tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Ink Speech-to-Text API
  slug: stt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-auth-api-openapi.yml
  format: yaml
  label: Cartesia Auth API
  slug: cartesia-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-auth-api-openapi.yml
- filename: cartesia-stt-api-openapi.yml
  format: yaml
  label: Cartesia STT API
  slug: cartesia-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-stt-api-openapi.yml
- filename: cartesia-tts-api-openapi.yml
  format: yaml
  label: Cartesia TTS API
  slug: cartesia-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-tts-api-openapi.yml
- filename: cartesia-voices-api-openapi.yml
  format: yaml
  label: Cartesia Voices API
  slug: cartesia-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-voices-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cartesia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cartesia secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cartesia
provider_slug: cartesia
scheme_count: 2
schemes:
- description: Cartesia API key (sk_car_...)
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/cartesia-openapi.yml
  type: apiKey
- description: Short-lived client access token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cartesia-openapi.yml
  type: http
slug: cartesia-authentication
source_filename: cartesia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cartesia-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Cartesia API key (sk_car_...)\n  sources:\n  - openapi/cartesia-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Short-lived client access token\n  sources:\n  - openapi/cartesia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/authentication/cartesia-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Voice
- TTS
- Text to Speech
- STT
- Speech to Text
- Streaming
- WebSocket
- Voice Agents
- Voice Clone
- Sonic
- Ink
- Real-Time
---
