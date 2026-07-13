---
api_key_in: []
api_specs:
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Speech API
  slug: unrealspeech-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Stream API
  slug: unrealspeech-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Synthesis Tasks API
  slug: unrealspeech-synthesis-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unrealspeech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unreal Speech secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unreal Speech
provider_slug: unrealspeech
scheme_count: 1
schemes:
- description: 'API key issued from the Unreal Speech dashboard, sent as Authorization: Bearer <API_KEY>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unrealspeech-openapi.yml
  type: http
slug: unrealspeech-authentication
source_filename: unrealspeech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unrealspeech-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued from the Unreal Speech dashboard, sent as Authorization: Bearer\n    <API_KEY>.'\n  sources:\n  - openapi/unrealspeech-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/authentication/unrealspeech-authentication.yml
summary_line: http · 1 scheme
tags:
- Text to Speech
- TTS
- Speech Synthesis
- Audio
- Voice
- AI
---
