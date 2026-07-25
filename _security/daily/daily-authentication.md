---
api_key_in: []
api_specs:
- filename: daily-batch-rooms-api-openapi.yml
  format: yaml
  label: Daily batch/rooms API
  slug: daily-batch-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-batch-rooms-api-openapi.yml
- filename: daily-dialin-api-openapi.yml
  format: yaml
  label: Daily dialin API
  slug: daily-dialin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-dialin-api-openapi.yml
- filename: daily-domain-api-openapi.yml
  format: yaml
  label: Daily domain API
  slug: daily-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-domain-api-openapi.yml
- filename: daily-domain-dialin-config-api-openapi.yml
  format: yaml
  label: Daily domain-dialin-config API
  slug: daily-domain-dialin-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-domain-dialin-config-api-openapi.yml
- filename: daily-logs-api-openapi.yml
  format: yaml
  label: Daily logs API
  slug: daily-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-logs-api-openapi.yml
- filename: daily-meeting-tokens-api-openapi.yml
  format: yaml
  label: Daily meeting-tokens API
  slug: daily-meeting-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-meeting-tokens-api-openapi.yml
- filename: daily-meetings-api-openapi.yml
  format: yaml
  label: Daily meetings API
  slug: daily-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-meetings-api-openapi.yml
- filename: daily-phone-numbers-api-openapi.yml
  format: yaml
  label: Daily phone-numbers API
  slug: daily-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-phone-numbers-api-openapi.yml
- filename: daily-presence-api-openapi.yml
  format: yaml
  label: Daily presence API
  slug: daily-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-presence-api-openapi.yml
- filename: daily-recordings-api-openapi.yml
  format: yaml
  label: Daily recordings API
  slug: daily-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-recordings-api-openapi.yml
- filename: daily-rooms-api-openapi.yml
  format: yaml
  label: Daily rooms API
  slug: daily-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-rooms-api-openapi.yml
- filename: daily-transcript-api-openapi.yml
  format: yaml
  label: Daily transcript API
  slug: daily-transcript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-transcript-api-openapi.yml
- filename: daily-webhooks-api-openapi.yml
  format: yaml
  label: Daily webhooks API
  slug: daily-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-webhooks-api-openapi.yml
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
