---
api_key_in: []
api_specs:
- filename: fastpix-data-api-openapi.yml
  format: yaml
  label: FastPix Data API
  slug: fastpix-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-data-api-openapi.yml
- filename: fastpix-drm-api-openapi.yml
  format: yaml
  label: FastPix DRM API
  slug: fastpix-drm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-drm-api-openapi.yml
- filename: fastpix-in-video-ai-api-openapi.yml
  format: yaml
  label: FastPix In-Video AI API
  slug: fastpix-in-video-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-in-video-ai-api-openapi.yml
- filename: fastpix-live-streaming-api-openapi.yml
  format: yaml
  label: FastPix Live Streaming API
  slug: fastpix-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-live-streaming-api-openapi.yml
- filename: fastpix-on-demand-api-openapi.yml
  format: yaml
  label: FastPix On-Demand API
  slug: fastpix-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-on-demand-api-openapi.yml
- filename: fastpix-playback-api-openapi.yml
  format: yaml
  label: FastPix Playback API
  slug: fastpix-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-playback-api-openapi.yml
- filename: fastpix-signing-keys-api-openapi.yml
  format: yaml
  label: FastPix Signing Keys API
  slug: fastpix-signing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-signing-keys-api-openapi.yml
- filename: fastpix-simulcast-api-openapi.yml
  format: yaml
  label: FastPix Simulcast API
  slug: fastpix-simulcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-simulcast-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fastpix Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastPix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FastPix
provider_slug: fastpix
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use your FastPix Access Token ID as the username and your Secret Key as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fastpix-openapi.yml
  type: http
slug: fastpix-authentication
source_filename: fastpix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fastpix-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use your FastPix Access Token ID as the username and\n    your Secret Key as the password.\n  sources:\n  - openapi/fastpix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/authentication/fastpix-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Live Streaming
- Video-on-Demand
- Encoding
- Playback
- Video Analytics
---
