---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mazdek-ai-account-limits-webhooks-api-openapi.yml
  format: yaml
  label: Mazdek AI Account, limits & webhooks API
  slug: mazdek-ai-account-limits-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-account-limits-webhooks-api-openapi.yml
- filename: mazdek-ai-songs-stran-api-openapi.yml
  format: yaml
  label: Mazdek AI Songs (Stran) API
  slug: mazdek-ai-songs-stran-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-songs-stran-api-openapi.yml
- filename: mazdek-ai-speech-to-text-asr-api-openapi.yml
  format: yaml
  label: Mazdek AI Speech-to-Text (ASR) API
  slug: mazdek-ai-speech-to-text-asr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-speech-to-text-asr-api-openapi.yml
- filename: mazdek-ai-spell-check-rastniv-s-api-openapi.yml
  format: yaml
  label: Mazdek AI Spell check (Rastnivîs) API
  slug: mazdek-ai-spell-check-rastniv-s-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-spell-check-rastniv-s-api-openapi.yml
- filename: mazdek-ai-text-to-speech-tts-api-openapi.yml
  format: yaml
  label: Mazdek AI Text-to-Speech (TTS) API
  slug: mazdek-ai-text-to-speech-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-text-to-speech-tts-api-openapi.yml
- filename: mazdek-ai-translation-api-openapi.yml
  format: yaml
  label: Mazdek AI Translation API
  slug: mazdek-ai-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-translation-api-openapi.yml
- filename: mazdek-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Mazdek AI Chat Completions API
  slug: mazdek-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mazdek-ai/openapi/mazdek-ai-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mazdek AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mazdek AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mazdek AI
provider_slug: mazdek-ai
scheme_count: 1
schemes:
- description: 'API key: Authorization: Bearer mazdek_sk_…'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mazdek-openapi.json
  type: http
slug: mazdek-ai-authentication
source_filename: mazdek-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mazdek-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key: Authorization: Bearer mazdek_sk_…'\n  sources:\n  - openapi/mazdek-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mazdek-ai/authentication/mazdek-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Kurdish
- Translation
- Speech
- Voice
---
