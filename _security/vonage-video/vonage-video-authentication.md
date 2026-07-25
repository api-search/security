---
api_key_in: []
api_specs:
- filename: vonage-video-archives-api-openapi.yml
  format: yaml
  label: Vonage Video API Archives API
  slug: vonage-video-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-archives-api-openapi.yml
- filename: vonage-video-broadcasts-api-openapi.yml
  format: yaml
  label: Vonage Video API Broadcasts API
  slug: vonage-video-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-broadcasts-api-openapi.yml
- filename: vonage-video-captions-api-openapi.yml
  format: yaml
  label: Vonage Video API Captions API
  slug: vonage-video-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-captions-api-openapi.yml
- filename: vonage-video-moderation-api-openapi.yml
  format: yaml
  label: Vonage Video API Moderation API
  slug: vonage-video-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-moderation-api-openapi.yml
- filename: vonage-video-render-api-openapi.yml
  format: yaml
  label: Vonage Video API Render API
  slug: vonage-video-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-render-api-openapi.yml
- filename: vonage-video-sessions-api-openapi.yml
  format: yaml
  label: Vonage Video API Sessions API
  slug: vonage-video-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-sessions-api-openapi.yml
- filename: vonage-video-signaling-api-openapi.yml
  format: yaml
  label: Vonage Video API Signaling API
  slug: vonage-video-signaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-signaling-api-openapi.yml
- filename: vonage-video-sip-api-openapi.yml
  format: yaml
  label: Vonage Video API SIP API
  slug: vonage-video-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-sip-api-openapi.yml
- filename: vonage-video-streams-api-openapi.yml
  format: yaml
  label: Vonage Video API Streams API
  slug: vonage-video-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-streams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vonage Video Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vonage Video API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vonage Video API
provider_slug: vonage-video
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A JWT generated from your Vonage application's private key and application ID, sent in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vonage-video-openapi.yml
  type: http
slug: vonage-video-authentication
source_filename: vonage-video-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vonage-video-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A JWT generated from your Vonage application's private key and application ID,\n    sent in the Authorization header.\n  sources:\n  - openapi/vonage-video-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/authentication/vonage-video-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- WebRTC
- Live Streaming
- Real-Time Communications
- CPaaS
---
