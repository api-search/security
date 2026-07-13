---
api_key_in:
- header
api_specs:
- filename: batch.yaml
  format: yaml
  label: Speechmatics Batch Transcription API
  slug: batch-transcription-api
  spec_type: OpenAPI
  url: https://docs.speechmatics.com/batch.yaml
- filename: speechmatics-management-api-openapi.yml
  format: yaml
  label: Speechmatics Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechmatics/refs/heads/main/openapi/speechmatics-management-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Speechmatics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speechmatics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Speechmatics
provider_slug: speechmatics
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Use the format: Bearer $API_KEY_OR_JWT'
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/speechmatics-batch-transcription-api-openapi.yml
  - openapi/speechmatics-management-api-openapi.yml
  type: apiKey
slug: speechmatics-authentication
source_filename: speechmatics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/speechmatics-batch-transcription-api-openapi.yml, openapi/speechmatics-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Bearer token authentication. Use the format: Bearer $API_KEY_OR_JWT'\n  sources:\n  - openapi/speechmatics-batch-transcription-api-openapi.yml\n  - openapi/speechmatics-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speechmatics/refs/heads/main/authentication/speechmatics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Speech Recognition
- Speech-to-Text
- Transcription
- Real-Time Transcription
- Batch Transcription
- Speaker Diarization
- Text-to-Speech
- Voice AI
- NLP
- Audio Processing
- WebSocket
- REST
---
