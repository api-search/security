---
api_key_in: []
api_specs:
- filename: whereby-insights-api-openapi.yml
  format: yaml
  label: Whereby Insights API
  slug: whereby-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-insights-api-openapi.yml
- filename: whereby-meetings-api-openapi.yml
  format: yaml
  label: Whereby Meetings API
  slug: whereby-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-meetings-api-openapi.yml
- filename: whereby-recordings-api-openapi.yml
  format: yaml
  label: Whereby Recordings API
  slug: whereby-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-recordings-api-openapi.yml
- filename: whereby-rooms-api-openapi.yml
  format: yaml
  label: Whereby Rooms API
  slug: whereby-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-rooms-api-openapi.yml
- filename: whereby-summaries-api-openapi.yml
  format: yaml
  label: Whereby Summaries API
  slug: whereby-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-summaries-api-openapi.yml
- filename: whereby-transcriptions-api-openapi.yml
  format: yaml
  label: Whereby Transcriptions API
  slug: whereby-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-transcriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Whereby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whereby secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whereby
provider_slug: whereby
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/whereby-openapi.yml
  type: http
slug: whereby-authentication
source_filename: whereby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whereby-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/whereby-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/authentication/whereby-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Communications
- Real-Time
- WebRTC
- Embedded
- Meetings
- Collaboration
---
