---
api_key_in: []
api_specs:
- filename: fish-audio-asr-api-openapi.yml
  format: yaml
  label: Fish Audio Asr API
  slug: fish-audio-asr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/openapi/fish-audio-asr-api-openapi.yml
- filename: fish-audio-model-api-openapi.yml
  format: yaml
  label: Fish Audio Model API
  slug: fish-audio-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/openapi/fish-audio-model-api-openapi.yml
- filename: fish-audio-tts-api-openapi.yml
  format: yaml
  label: Fish Audio Tts API
  slug: fish-audio-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/openapi/fish-audio-tts-api-openapi.yml
- filename: fish-audio-wallet-api-openapi.yml
  format: yaml
  label: Fish Audio Wallet API
  slug: fish-audio-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/openapi/fish-audio-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fish Audio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fish Audio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fish Audio
provider_slug: fish-audio
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fish-audio-openapi.yml
  type: http
slug: fish-audio-authentication
source_filename: fish-audio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fish-audio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fish-audio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/authentication/fish-audio-authentication.yml
summary_line: http · 1 scheme
tags:
- Voice
- Text to Speech
- Speech to Text
- Voice Cloning
- Audio
- Generative AI
- Multilingual
- Streaming
- SDK
- Open Source
---
