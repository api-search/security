---
api_key_in: []
api_specs:
- filename: bytark-live-api-openapi.yml
  format: yaml
  label: ByteArk Live API
  slug: bytark-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-live-api-openapi.yml
- filename: bytark-uploads-api-openapi.yml
  format: yaml
  label: ByteArk Uploads API
  slug: bytark-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-uploads-api-openapi.yml
- filename: bytark-videos-api-openapi.yml
  format: yaml
  label: ByteArk Videos API
  slug: bytark-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bytark Authentication
name_suffix: Authentication
oauth_flows: []
overview: ByteArk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ByteArk
provider_slug: bytark
scheme_count: 1
schemes:
- description: 'Personal access token passed as `Authorization: Bearer <token>`. Tokens are generated in the ByteArk Personal Access Token settings. Fleet live channel endpoints instead authenticate with a serviceId / apiKey path pair.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bytark-openapi.yml
  type: http
slug: bytark-authentication
source_filename: bytark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bytark-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token passed as `Authorization: Bearer <token>`. Tokens are\n    generated in the ByteArk Personal Access Token settings. Fleet live channel endpoints instead\n    authenticate with a serviceId / apiKey path pair.'\n  sources:\n  - openapi/bytark-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/authentication/bytark-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Video-on-Demand
- Live Streaming
- CDN
- Object Storage
- Transcoding
- DRM
- Media
---
