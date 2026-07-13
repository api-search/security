---
api_key_in: []
api_specs:
- filename: 100ms-live-server-side-api-openapi.yml
  format: yaml
  label: 100ms Server-Side API
  slug: server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/openapi/100ms-live-server-side-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 100Ms Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: 100ms secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 100ms
provider_slug: 100ms-live
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Short-lived HS256 JWT generated server-side from the app access key/secret downloaded from the 100ms dashboard. Include as `Authorization: Bearer <token>`.'
  name: ManagementToken
  scheme: bearer
  sources:
  - openapi/100ms-live-server-side-api-openapi.yml
  type: http
slug: 100ms-live-authentication
source_filename: 100ms-live-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/100ms-live-server-side-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ManagementToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Short-lived HS256 JWT generated server-side from the app access key/secret downloaded\n    from the 100ms dashboard. Include as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/100ms-live-server-side-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/authentication/100ms-live-authentication.yml
summary_line: http · 1 scheme
tags:
- Live Video
- Live Streaming
- Video Conferencing
- WebRTC
- HLS
- RTMP
- Recording
- Real-time Messaging
- Live Infrastructure
- India
---
