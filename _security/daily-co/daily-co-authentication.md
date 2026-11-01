---
anonymous_access: false
api_key_in: []
api_specs:
- filename: daily-co-domain-api-openapi.yml
  format: yaml
  label: Daily Domain API
  slug: daily-co-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-domain-api-openapi.yml
- filename: daily-co-meetings-api-openapi.yml
  format: yaml
  label: Daily Meetings API
  slug: daily-co-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-meetings-api-openapi.yml
- filename: daily-co-presence-api-openapi.yml
  format: yaml
  label: Daily Presence API
  slug: daily-co-presence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-presence-api-openapi.yml
- filename: daily-co-recordings-api-openapi.yml
  format: yaml
  label: Daily Recordings API
  slug: daily-co-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-recordings-api-openapi.yml
- filename: daily-co-rooms-api-openapi.yml
  format: yaml
  label: Daily Rooms API
  slug: daily-co-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-rooms-api-openapi.yml
- filename: daily-co-webhooks-api-openapi.yml
  format: yaml
  label: Daily Webhooks API
  slug: daily-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-webhooks-api-openapi.yml
- filename: daily-co-meeting-tokens-api-openapi.yml
  format: yaml
  label: Daily Meeting Tokens API
  slug: daily-co-meeting-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-meeting-tokens-api-openapi.yml
- filename: daily-co-phone-numbers-api-openapi.yml
  format: yaml
  label: Daily Phone Numbers API
  slug: daily-co-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-phone-numbers-api-openapi.yml
- filename: daily-co-batch-rooms-api-openapi.yml
  format: yaml
  label: Daily Batch/rooms API
  slug: daily-co-batch-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-batch-rooms-api-openapi.yml
- filename: daily-co-domain-dialin-config-api-openapi.yml
  format: yaml
  label: Daily Domain Dialin Config API
  slug: daily-co-domain-dialin-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-domain-dialin-config-api-openapi.yml
- filename: daily-co-logs-api-openapi.yml
  format: yaml
  label: Daily Logs API
  slug: daily-co-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-logs-api-openapi.yml
- filename: daily-co-transcript-api-openapi.yml
  format: yaml
  label: Daily Transcript API
  slug: daily-co-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-transcript-api-openapi.yml
- filename: daily-co-dial-in-api-openapi.yml
  format: yaml
  label: Daily Dial In API
  slug: daily-co-dial-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-co/openapi/daily-co-dial-in-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/daily-co/authentication/daily-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Daily
- Real-Time
- WebRTC
- Video
- Audio
- SDK
- Voice AI
- Recording
- Transcription
- Voice
---
