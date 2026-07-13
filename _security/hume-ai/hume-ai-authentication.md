---
api_key_in:
- header
api_specs:
- filename: hume-ai-voices-openapi.yml
  format: yaml
  label: Hume Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-voices-openapi.yml
- filename: hume-ai-tts-openapi.yml
  format: yaml
  label: Hume Octave Text-to-Speech API
  slug: tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-tts-openapi.yml
- filename: hume-ai-evi-openapi.yml
  format: yaml
  label: Hume Empathic Voice Interface (EVI) API
  slug: evi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-evi-openapi.yml
- filename: hume-ai-expression-openapi.yml
  format: yaml
  label: Hume Expression Measurement API
  slug: expression
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-expression-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hume Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hume AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hume AI
provider_slug: hume-ai
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: X-Hume-Api-Key
  sources:
  - openapi/hume-ai-evi-openapi.yml
  - openapi/hume-ai-expression-openapi.yml
  - openapi/hume-ai-tts-openapi.yml
  - openapi/hume-ai-voices-openapi.yml
  type: apiKey
slug: hume-ai-authentication
source_filename: hume-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hume-ai-evi-openapi.yml, openapi/hume-ai-expression-openapi.yml, openapi/hume-ai-tts-openapi.yml,\n  openapi/hume-ai-voices-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: X-Hume-Api-Key\n  sources:\n  - openapi/hume-ai-evi-openapi.yml\n  - openapi/hume-ai-expression-openapi.yml\n  - openapi/hume-ai-tts-openapi.yml\n  - openapi/hume-ai-voices-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/authentication/hume-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Voice
- Empathic
- Emotion
- Multimodal
---
