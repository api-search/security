---
api_key_in: []
api_specs:
- filename: inworld-tts-api-openapi.yml
  format: yaml
  label: Inworld TTS API
  slug: inworld-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-tts-api-openapi.yml
- filename: inworld-voice-api-openapi.yml
  format: yaml
  label: Inworld Voice API
  slug: inworld-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-voice-api-openapi.yml
- filename: inworld-stt-api-openapi.yml
  format: yaml
  label: Inworld STT API
  slug: inworld-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-stt-api-openapi.yml
- filename: inworld-realtime-api-openapi.yml
  format: yaml
  label: Inworld Realtime API
  slug: inworld-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-realtime-api-openapi.yml
- filename: inworld-router-api-openapi.yml
  format: yaml
  label: Inworld LLM Router API
  slug: inworld-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-router-api-openapi.yml
- filename: inworld-models-api-openapi.yml
  format: yaml
  label: Inworld Models API
  slug: inworld-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inworld Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inworld AI secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Inworld AI
provider_slug: inworld-ai
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/inworld-models-api-openapi.yml
  - openapi/inworld-stt-api-openapi.yml
  - openapi/inworld-tts-api-openapi.yml
  - openapi/inworld-voice-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/inworld-realtime-api-openapi.yml
  type: http
slug: inworld-ai-authentication
source_filename: inworld-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inworld-models-api-openapi.yml, openapi/inworld-realtime-api-openapi.yml, openapi/inworld-stt-api-openapi.yml,\n  openapi/inworld-tts-api-openapi.yml, openapi/inworld-voice-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/inworld-models-api-openapi.yml\n  - openapi/inworld-stt-api-openapi.yml\n  - openapi/inworld-tts-api-openapi.yml\n  - openapi/inworld-voice-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/inworld-realtime-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/authentication/inworld-ai-authentication.yml
summary_line: http · 2 schemes
tags:
- AI
- Artificial Intelligence
- Voice
- Text To Speech
- Speech To Text
- Realtime
- LLM Routing
- Voice Cloning
- Conversational AI
- Game AI
---
