---
api_key_in:
- query
api_specs:
- filename: red5-webrtc-streaming-asyncapi.yml
  format: yaml
  label: Red5 Pro WebRTC SDK
  slug: webrtc-sdk
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/asyncapi/red5-webrtc-streaming-asyncapi.yml
- filename: red5-admin-api-openapi.yml
  format: yaml
  label: Red5 Admin API
  slug: red5-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-admin-api-openapi.yml
- filename: red5-file-restreamer-api-openapi.yml
  format: yaml
  label: Red5 File Restreamer API
  slug: red5-file-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-file-restreamer-api-openapi.yml
- filename: red5-images-api-openapi.yml
  format: yaml
  label: Red5 Images API
  slug: red5-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-images-api-openapi.yml
- filename: red5-inputs-api-openapi.yml
  format: yaml
  label: Red5 Inputs API
  slug: red5-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-inputs-api-openapi.yml
- filename: red5-mixers-api-openapi.yml
  format: yaml
  label: Red5 Mixers API
  slug: red5-mixers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-mixers-api-openapi.yml
- filename: red5-provision-api-openapi.yml
  format: yaml
  label: Red5 Provision API
  slug: red5-provision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-provision-api-openapi.yml
- filename: red5-proxy-api-openapi.yml
  format: yaml
  label: Red5 Proxy API
  slug: red5-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-proxy-api-openapi.yml
- filename: red5-rtmp-restreamer-api-openapi.yml
  format: yaml
  label: Red5 RTMP Restreamer API
  slug: red5-rtmp-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-rtmp-restreamer-api-openapi.yml
- filename: red5-servlet-configuration-api-openapi.yml
  format: yaml
  label: Red5 Servlet Configuration API
  slug: red5-servlet-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-servlet-configuration-api-openapi.yml
- filename: red5-streams-api-openapi.yml
  format: yaml
  label: Red5 Streams API
  slug: red5-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-streams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Red5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red5 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red5
provider_slug: red5
scheme_count: 2
schemes:
- description: API access token for authenticating Brew Mixer API requests
  in: query
  name: accessToken
  parameter: accessToken
  sources:
  - openapi/red5-brew-mixer-api-openapi.yml
  - openapi/red5-restreamer-api-openapi.yml
  - openapi/red5-server-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT bearer token for authenticating Stream Manager API requests
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/red5-stream-manager-2-openapi.yml
  type: http
slug: red5-authentication
source_filename: red5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red5-brew-mixer-api-openapi.yml, openapi/red5-restreamer-api-openapi.yml, openapi/red5-server-api-openapi.yml,\n  openapi/red5-stream-manager-2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: API access token for authenticating Brew Mixer API requests\n  sources:\n  - openapi/red5-brew-mixer-api-openapi.yml\n  - openapi/red5-restreamer-api-openapi.yml\n  - openapi/red5-server-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token for authenticating Stream Manager API requests\n  sources:\n  - openapi/red5-stream-manager-2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/authentication/red5-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Live Streaming
- Media
- Real-Time
- RTMP
- Streaming
- Video
- WebRTC
---
