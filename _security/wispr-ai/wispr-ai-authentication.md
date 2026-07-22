---
api_key_in:
- header
api_specs:
- filename: wispr-ai-backend-openapi-original.json
  format: json
  label: Wispr Flow Backend API
  slug: wispr-flow-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wispr-ai/refs/heads/main/openapi/wispr-ai-backend-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wispr Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wispr AI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wispr AI
provider_slug: wispr-ai
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeaderPatched
  parameter: Authorization
  sources:
  - openapi/wispr-ai-backend-openapi-original.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/wispr-ai-backend-openapi-original.json
  type: apiKey
slug: wispr-ai-authentication
source_filename: wispr-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wispr-ai-backend-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeaderPatched\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/wispr-ai-backend-openapi-original.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/wispr-ai-backend-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wispr-ai/refs/heads/main/authentication/wispr-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Voice
- Speech-to-Text
- Dictation
- Artificial Intelligence
- Productivity
- Transcription
---
