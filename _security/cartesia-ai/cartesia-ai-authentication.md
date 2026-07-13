---
api_key_in: []
api_specs:
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Text-to-Speech API
  slug: cartesia-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-asyncapi.yml
  format: yaml
  label: Cartesia TTS WebSocket API
  slug: cartesia-ai-tts-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/asyncapi/cartesia-ai-asyncapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Speech-to-Text API
  slug: cartesia-ai-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-asyncapi.yml
  format: yaml
  label: Cartesia STT WebSocket API
  slug: cartesia-ai-stt-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/asyncapi/cartesia-ai-asyncapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voices API
  slug: cartesia-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voice Changer API
  slug: cartesia-ai-voice-changer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Infill API
  slug: cartesia-ai-infill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Datasets API
  slug: cartesia-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Pronunciation Dictionaries API
  slug: cartesia-ai-pronunciation-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia API Keys and Auth API
  slug: cartesia-ai-api-keys-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voice Agents API
  slug: cartesia-ai-voice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Usage API
  slug: cartesia-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cartesia Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cartesia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cartesia
provider_slug: cartesia-ai
scheme_count: 1
schemes:
- bearerFormat: sk_car_... API key or short-lived access token
  description: 'Cartesia API key (sk_car_...) or a short-lived access token minted via POST /access-token, passed as Authorization: Bearer <token>. Every request also requires the Cartesia-Version header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cartesia-ai-openapi.yml
  type: http
slug: cartesia-ai-authentication
source_filename: cartesia-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cartesia-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_car_... API key or short-lived access token\n  description: 'Cartesia API key (sk_car_...) or a short-lived access token minted via POST\n    /access-token, passed as Authorization: Bearer <token>. Every request also requires the\n    Cartesia-Version header.'\n  sources:\n  - openapi/cartesia-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/authentication/cartesia-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice AI
- Text to Speech
- Speech to Text
- Realtime
- WebSocket
- Voice Cloning
- Voice Agents
---
