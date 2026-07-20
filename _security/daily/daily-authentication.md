---
api_key_in: []
api_specs:
- filename: daily-openapi-original.json
  format: json
  label: Daily API
  slug: daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Daily Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daily secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Daily
provider_slug: daily
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/daily-openapi-original.json
  type: http
slug: daily-authentication
source_filename: daily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/daily-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/daily-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/authentication/daily-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Audio
- WebRTC
- Real-Time Communication
- Video Conferencing
- Live Streaming
- Recording
- Transcription
- Telephony
- SIP
- PSTN
- Company
---
