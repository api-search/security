---
api_key_in:
- header
api_specs:
- filename: deepgram-speech-to-text-openapi.yml
  format: yaml
  label: Deepgram Speech-To-Text API
  slug: speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-speech-to-text-openapi.yml
- filename: deepgram-text-to-speech-openapi.yml
  format: yaml
  label: Deepgram Text-To-Speech API
  slug: text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-to-speech-openapi.yml
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-speech-to-text-openapi.yml
  format: yaml
  label: Deepgram Audio Intelligence API
  slug: audio-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-speech-to-text-openapi.yml
- filename: deepgram-management-openapi.yml
  format: yaml
  label: Deepgram Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-management-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepgram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepgram secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Deepgram
provider_slug: deepgram
scheme_count: 2
schemes:
- description: Deepgram API key passed as a bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepgram-management-openapi.yml
  - openapi/deepgram-speech-to-text-openapi.yml
  - openapi/deepgram-text-to-speech-openapi.yml
  type: http
- description: Deepgram API key passed with Token prefix, e.g. Token YOUR_API_KEY.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/deepgram-speech-to-text-openapi.yml
  type: apiKey
slug: deepgram-authentication
source_filename: deepgram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepgram-management-openapi.yml, openapi/deepgram-speech-to-text-openapi.yml,\n  openapi/deepgram-text-to-speech-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Deepgram API key passed as a bearer token in the Authorization header.\n  sources:\n  - openapi/deepgram-management-openapi.yml\n  - openapi/deepgram-speech-to-text-openapi.yml\n  - openapi/deepgram-text-to-speech-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Deepgram API key passed with Token prefix, e.g. Token YOUR_API_KEY.\n  sources:\n  - openapi/deepgram-speech-to-text-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/authentication/deepgram-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Speech-To-Text
- Text-To-Speech
- Transcription
- Voice AI
---
