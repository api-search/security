---
api_key_in: []
api_specs:
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Text-to-Speech (Waves)
  slug: text-to-speech-waves
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Streaming / Realtime TTS
  slug: streaming-realtime-tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Voices / Cloning
  slug: voices-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smallest Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smallest AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smallest AI
provider_slug: smallest-ai
scheme_count: 1
schemes:
- description: 'Pass your Waves API key as a Bearer token in the Authorization header: `Authorization: Bearer <SMALLEST_API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smallest-ai-openapi.yml
  type: http
slug: smallest-ai-authentication
source_filename: smallest-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smallest-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your Waves API key as a Bearer token in the Authorization header: `Authorization:\n    Bearer <SMALLEST_API_KEY>`.'\n  sources:\n  - openapi/smallest-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/authentication/smallest-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Text to Speech
- Voice
- Realtime
- Voice Agents
---
