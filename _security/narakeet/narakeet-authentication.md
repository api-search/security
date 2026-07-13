---
api_key_in:
- header
api_specs:
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Text to Speech API
  slug: narakeet-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Markdown to Video API
  slug: narakeet-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Voice Listing API
  slug: narakeet-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Account Credits API
  slug: narakeet-account-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Narakeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Narakeet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Narakeet
provider_slug: narakeet
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/narakeet-openapi.yml
  type: apiKey
slug: narakeet-authentication
source_filename: narakeet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/narakeet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/narakeet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/authentication/narakeet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Text to Speech
- TTS
- Voice
- Audio
- Video
- AI
- Media Generation
---
