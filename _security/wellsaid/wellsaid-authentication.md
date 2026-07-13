---
api_key_in:
- header
api_specs:
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Text-to-Speech API
  slug: wellsaid-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Streaming TTS API
  slug: wellsaid-streaming-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Voices and Speakers API
  slug: wellsaid-voices-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wellsaid Authentication
name_suffix: Authentication
oauth_flows: []
overview: WellSaid Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WellSaid Labs
provider_slug: wellsaid
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/wellsaid-openapi.yml
  type: apiKey
slug: wellsaid-authentication
source_filename: wellsaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellsaid-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/wellsaid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/authentication/wellsaid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Text to Speech
- Voice
- Audio
- TTS
---
