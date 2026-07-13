---
api_key_in:
- header
api_specs:
- filename: videosdk-realtime-communication-api-openapi.yml
  format: yaml
  label: VideoSDK Real-Time Communication API
  slug: realtime-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videosdk/refs/heads/main/openapi/videosdk-realtime-communication-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Videosdk Authentication
name_suffix: Authentication
oauth_flows: []
overview: VideoSDK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VideoSDK
provider_slug: videosdk
scheme_count: 1
schemes:
- description: JWT token generated using your VideoSDK API key and secret (HS256). Pass the token directly without a "Bearer" prefix.
  in: header
  name: JWTAuth
  parameter: Authorization
  sources:
  - openapi/videosdk-realtime-communication-api-openapi.yml
  type: apiKey
slug: videosdk-authentication
source_filename: videosdk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/videosdk-realtime-communication-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: JWTAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT token generated using your VideoSDK API key and secret (HS256). Pass the\n    token directly without a \"Bearer\" prefix.\n  sources:\n  - openapi/videosdk-realtime-communication-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videosdk/refs/heads/main/authentication/videosdk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video
- Audio
- WebRTC
- Real-Time Communication
- Live Streaming
- HLS
- RTMP
- AI Agents
- Video Conferencing
- WebSocket
---
