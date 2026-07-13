---
api_key_in:
- header
api_specs:
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Text-to-Speech API
  slug: camb-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Dubbing API
  slug: camb-ai-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Translation API
  slug: camb-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Voices API
  slug: camb-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Transcription API
  slug: camb-ai-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Camb Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Camb.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Camb.AI
provider_slug: camb-ai
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/camb-ai-openapi.yml
  type: apiKey
slug: camb-ai-authentication
source_filename: camb-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camb-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/camb-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/authentication/camb-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Text to Speech
- Dubbing
- Translation
- Transcription
- Voice Cloning
- Speech
---
