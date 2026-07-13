---
api_key_in:
- header
api_specs:
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Text-to-Speech API
  slug: wellsaid-labs-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Clips API
  slug: wellsaid-labs-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Voice Avatars API
  slug: wellsaid-labs-voice-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Pronunciation API
  slug: wellsaid-labs-pronunciation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wellsaid Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: WellSaid Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WellSaid Labs
provider_slug: wellsaid-labs
scheme_count: 1
schemes:
- description: API key issued by WellSaid Labs, passed in the X-Api-Key header. Request a trial key from the console; production use requires a business plan.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/wellsaid-labs-openapi.yml
  type: apiKey
slug: wellsaid-labs-authentication
source_filename: wellsaid-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellsaid-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key issued by WellSaid Labs, passed in the X-Api-Key header. Request a trial\n    key from the console; production use requires a business plan.\n  sources:\n  - openapi/wellsaid-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/authentication/wellsaid-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Text to Speech
- TTS
- Voice
- Voiceover
- Speech Synthesis
- Audio
---
