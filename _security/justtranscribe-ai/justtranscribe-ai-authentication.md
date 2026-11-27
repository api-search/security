---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justtranscribe-ai-me-api-openapi.yml
  format: yaml
  label: JustTranscribe Me API
  slug: justtranscribe-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justtranscribe-ai/openapi/justtranscribe-ai-me-api-openapi.yml
- filename: justtranscribe-ai-transcripts-api-openapi.yml
  format: yaml
  label: JustTranscribe Transcripts API
  slug: justtranscribe-ai-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justtranscribe-ai/openapi/justtranscribe-ai-transcripts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustTranscribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustTranscribe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustTranscribe
provider_slug: justtranscribe-ai
scheme_count: 1
schemes:
- description: API key from https://justtranscribe.ai/api-keys (jt_live_…).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/justtranscribe-ai-openapi.json
  type: http
slug: justtranscribe-ai-authentication
source_filename: justtranscribe-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justtranscribe-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from https://justtranscribe.ai/api-keys (jt_live_…).\n  sources:\n  - openapi/justtranscribe-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/justtranscribe-ai/authentication/justtranscribe-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Transcription
- Audio
- Video
- Artificial Intelligence
- Free
- Software-as-a-Service
---
