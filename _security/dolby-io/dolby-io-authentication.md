---
api_key_in: []
api_specs:
- filename: dolby-io-realtime-streaming-api-openapi.yml
  format: yaml
  label: Dolby OptiView Real-time Streaming API
  slug: dolby-io-realtime-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-realtime-streaming-api-openapi.yml
- filename: swagger.json
  format: json
  label: Dolby OptiView Live (THEOlive) API
  slug: dolby-io-theolive-api
  spec_type: OpenAPI
  url: https://api.theo.live/v2/api-docs/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dolby Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dolby.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dolby.io
provider_slug: dolby-io
scheme_count: 2
schemes:
- bearerFormat: API Secret
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dolby-io-realtime-streaming-api-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/dolby-io-theolive-api-openapi.yml
  type: http
slug: dolby-io-authentication
source_filename: dolby-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dolby-io-realtime-streaming-api-openapi.yml, openapi/dolby-io-theolive-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Secret\n  sources:\n  - openapi/dolby-io-realtime-streaming-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dolby-io-theolive-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/authentication/dolby-io-authentication.yml
summary_line: http · 2 schemes
tags:
- Media
- Streaming
- Real-time Streaming
- WebRTC
- Live Streaming
- Low Latency
- Video
- Audio
- Broadcast
- Player
- Advertising
- Dolby OptiView
- Millicast
- THEOlive
- THEOplayer
---
