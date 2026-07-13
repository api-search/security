---
api_key_in:
- header
api_specs:
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Text-to-Speech API
  slug: lovo-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Speakers API
  slug: lovo-ai-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Pronunciation and Prosody
  slug: lovo-ai-pronunciation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Teams and Billing API
  slug: lovo-ai-teams-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lovo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LOVO AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LOVO AI
provider_slug: lovo-ai
scheme_count: 1
schemes:
- description: API key generated at https://genny.lovo.ai (profile tab).
  in: header
  name: X-API-KEY
  parameter: X-API-KEY
  sources:
  - openapi/lovo-ai-openapi.yml
  type: apiKey
slug: lovo-ai-authentication
source_filename: lovo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lovo-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key generated at https://genny.lovo.ai (profile tab).\n  sources:\n  - openapi/lovo-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/authentication/lovo-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Text to Speech
- TTS
- Voice Generation
- Voice Cloning
- Speech Synthesis
- Voiceover
---
