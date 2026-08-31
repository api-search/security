---
api_key_in: []
api_specs:
- filename: uberduck-conversational-api-openapi.yml
  format: yaml
  label: Uberduck Conversational API
  slug: uberduck-conversational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-conversational-api-openapi.yml
- filename: uberduck-models-api-openapi.yml
  format: yaml
  label: Uberduck Models API
  slug: uberduck-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-models-api-openapi.yml
- filename: uberduck-text-to-speech-api-openapi.yml
  format: yaml
  label: Uberduck Text-to-Speech API
  slug: uberduck-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-text-to-speech-api-openapi.yml
- filename: uberduck-voices-api-openapi.yml
  format: yaml
  label: Uberduck Voices API
  slug: uberduck-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-voices-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uberduck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uberduck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uberduck
provider_slug: uberduck
scheme_count: 1
schemes:
- description: Bearer API key generated in Uberduck account settings under the API section.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/uberduck-openapi.yml
  type: http
slug: uberduck-authentication
source_filename: uberduck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uberduck-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: Bearer API key generated in Uberduck account settings under the API section.\n  sources:\n  - openapi/uberduck-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/authentication/uberduck-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Text to Speech
- TTS
- Voice
- Voice Cloning
- Speech Synthesis
- Conversational AI
---
