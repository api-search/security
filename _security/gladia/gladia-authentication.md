---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Gladia Live (Real-time) API
  slug: gladia-live-real-time-api
  spec_type: AsyncAPI
  url: https://github.com/gladiaio/docs
- filename: gladia-audiototext-api-openapi.yml
  format: yaml
  label: Gladia AudioToText API
  slug: gladia-audiototext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-audiototext-api-openapi.yml
- filename: gladia-file-management-api-openapi.yml
  format: yaml
  label: Gladia File Management API
  slug: gladia-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-file-management-api-openapi.yml
- filename: gladia-job-history-api-openapi.yml
  format: yaml
  label: Gladia Job History API
  slug: gladia-job-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-job-history-api-openapi.yml
- filename: gladia-live-v2-api-openapi.yml
  format: yaml
  label: Gladia Live V2 API
  slug: gladia-live-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-live-v2-api-openapi.yml
- filename: gladia-openrouter-api-openapi.yml
  format: yaml
  label: Gladia OpenRouter API
  slug: gladia-openrouter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-openrouter-api-openapi.yml
- filename: gladia-pre-recorded-v2-api-openapi.yml
  format: yaml
  label: Gladia Pre-recorded V2 API
  slug: gladia-pre-recorded-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-pre-recorded-v2-api-openapi.yml
- filename: gladia-transcription-v1-api-openapi.yml
  format: yaml
  label: Gladia Transcription V1 API
  slug: gladia-transcription-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-transcription-v1-api-openapi.yml
- filename: gladia-transcription-v2-api-openapi.yml
  format: yaml
  label: Gladia Transcription V2 API
  slug: gladia-transcription-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/openapi/gladia-transcription-v2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gladia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gladia secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gladia
provider_slug: gladia
scheme_count: 1
schemes:
- description: Your personal Gladia API key
  in: header
  name: x_gladia_key
  parameter: x-gladia-key
  sources:
  - openapi/gladia-control-api-openapi.yml
  type: apiKey
slug: gladia-authentication
source_filename: gladia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gladia-control-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x_gladia_key\n  type: apiKey\n  in: header\n  parameter: x-gladia-key\n  description: Your personal Gladia API key\n  sources:\n  - openapi/gladia-control-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/authentication/gladia-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Speech-to-Text
- Transcription
- Audio Intelligence
- Real-Time
- Speaker Diarization
- Translation
- WebSocket
- REST
---
