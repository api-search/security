---
api_key_in:
- header
api_specs:
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Text-to-Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Podcastle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Podcastle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Podcastle
provider_slug: podcastle
scheme_count: 1
schemes:
- description: API key issued from the Async developer console.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/podcastle-openapi.yml
  type: apiKey
slug: podcastle-authentication
source_filename: podcastle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podcastle-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued from the Async developer console.\n  sources:\n  - openapi/podcastle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/authentication/podcastle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Audio
- Text to Speech
- Voice Cloning
- Podcasting
---
