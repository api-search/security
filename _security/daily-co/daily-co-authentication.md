---
api_key_in: []
api_specs:
- filename: daily-co-openapi.yml
  format: yaml
  label: Daily REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily-co/refs/heads/main/openapi/daily-co-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Daily Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daily secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Daily
provider_slug: daily-co
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/daily-co-openapi.yml
  type: http
slug: daily-co-authentication
source_filename: daily-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/daily-co-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/daily-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily-co/refs/heads/main/authentication/daily-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Realtime
- WebRTC
- Video
- Audio
- SDK
- Voice AI
- Recording
- Transcription
---
