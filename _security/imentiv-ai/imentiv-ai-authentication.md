---
api_key_in:
- header
api_specs:
- filename: imentiv-ai-ai-insights-api-api-openapi.yml
  format: yaml
  label: Imentiv AI AI Insights API API
  slug: imentiv-ai-ai-insights-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-ai-insights-api-api-openapi.yml
- filename: imentiv-ai-audio-emotion-api-api-openapi.yml
  format: yaml
  label: Imentiv AI Audio Emotion API API
  slug: imentiv-ai-audio-emotion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-audio-emotion-api-api-openapi.yml
- filename: imentiv-ai-image-emotion-api-api-openapi.yml
  format: yaml
  label: Imentiv AI Image Emotion API API
  slug: imentiv-ai-image-emotion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-image-emotion-api-api-openapi.yml
- filename: imentiv-ai-report-api-api-openapi.yml
  format: yaml
  label: Imentiv AI Report API API
  slug: imentiv-ai-report-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-report-api-api-openapi.yml
- filename: imentiv-ai-text-emotion-api-api-openapi.yml
  format: yaml
  label: Imentiv AI Text Emotion API API
  slug: imentiv-ai-text-emotion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-text-emotion-api-api-openapi.yml
- filename: imentiv-ai-video-emotion-api-api-openapi.yml
  format: yaml
  label: Imentiv AI Video Emotion API API
  slug: imentiv-ai-video-emotion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/openapi/imentiv-ai-video-emotion-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Imentiv Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imentiv AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Imentiv AI
provider_slug: imentiv-ai
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/imentiv-ai-openapi.yml
  type: apiKey
slug: imentiv-ai-authentication
source_filename: imentiv-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imentiv-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/imentiv-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/authentication/imentiv-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Emotion Detection
- Machine Learning
- Video Analysis
---
