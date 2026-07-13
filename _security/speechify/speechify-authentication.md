---
api_key_in: []
api_specs:
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Text-to-Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Streaming TTS API
  slug: streaming-tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Speechify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speechify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Speechify
provider_slug: speechify
scheme_count: 1
schemes:
- description: 'Pass your Speechify API key as a Bearer token in the Authorization header, e.g. "Authorization: Bearer $SPEECHIFY_API_KEY".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/speechify-openapi.yml
  type: http
slug: speechify-authentication
source_filename: speechify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/speechify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your Speechify API key as a Bearer token in the Authorization header, e.g.\n    \"Authorization: Bearer $SPEECHIFY_API_KEY\".'\n  sources:\n  - openapi/speechify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/authentication/speechify-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Text to Speech
- Voice
- Speech Synthesis
- Voice Cloning
---
