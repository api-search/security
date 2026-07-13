---
api_key_in:
- header
api_specs:
- filename: heygen-openapi.yml
  format: yaml
  label: HeyGen API
  slug: heygen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Heygen Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeyGen secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HeyGen
provider_slug: heygen
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/heygen-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/heygen-openapi.yml
  type: apiKey
slug: heygen-authentication
source_filename: heygen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heygen-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/heygen-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/heygen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/authentication/heygen-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Generative AI
- Video
- Avatars
- Voice Cloning
- Text To Speech
- Lipsync
- Translation
- Streaming
- MCP
---
