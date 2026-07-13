---
api_key_in: []
api_specs:
- filename: wowza-video-openapi.yml
  format: yaml
  label: Wowza Video REST API
  slug: wowza-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/openapi/wowza-video-openapi.yml
- filename: wowza-streaming-engine-openapi.yml
  format: yaml
  label: Wowza Streaming Engine REST API
  slug: wowza-streaming-engine-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/openapi/wowza-streaming-engine-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wowza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wowza secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wowza
provider_slug: wowza
scheme_count: 3
schemes:
- description: HTTP Basic Authentication using Wowza Streaming Engine admin credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wowza-streaming-engine-openapi.yml
  type: http
- description: HTTP Digest Authentication
  name: digestAuth
  scheme: digest
  sources:
  - openapi/wowza-streaming-engine-openapi.yml
  type: http
- description: Your Wowza-generated access token, also called a JSON web token (JWT). Send it as a bearer token in the Authentication header of your requests. See [Authentication](https://www.wowza.com/docs/how-to-use-the-wowza-video-rest-api#authentication).
  name: WV_JWT
  scheme: bearer
  sources:
  - openapi/wowza-video-openapi.yml
  type: http
slug: wowza-authentication
source_filename: wowza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wowza-streaming-engine-openapi.yml, openapi/wowza-video-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Wowza Streaming Engine admin credentials\n  sources:\n  - openapi/wowza-streaming-engine-openapi.yml\n- name: digestAuth\n  type: http\n  scheme: digest\n  description: HTTP Digest Authentication\n  sources:\n  - openapi/wowza-streaming-engine-openapi.yml\n- name: WV_JWT\n  type: http\n  scheme: bearer\n  description: Your Wowza-generated access token, also called a JSON web token (JWT). Send it\n    as a bearer token in the Authentication header of your requests. See [Authentication](https://www.wowza.com/docs/how-to-use-the-wowza-video-rest-api#authentication).\n  sources:\n  - openapi/wowza-video-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/authentication/wowza-authentication.yml
summary_line: http · 3 schemes
tags:
- Video
- Streaming
- Live Streaming
- Video On Demand
- Transcoding
- Media Server
- RTMP
- RTSP
- SRT
- WebRTC
- HLS
- MPEG-DASH
- Real-Time Streaming
- Low Latency
- Video Player
- HTML5 Player
- DRM
- CDN
- Video Analytics
- QoE
- Webhooks
- Edge
- Surveillance
- OTT
---
