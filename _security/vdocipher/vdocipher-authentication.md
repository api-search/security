---
api_key_in:
- header
api_specs:
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Videos API
  slug: vdocipher-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Upload API
  slug: vdocipher-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher OTP & Playback Credentials API
  slug: vdocipher-playback-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Folders API
  slug: vdocipher-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Watermark API
  slug: vdocipher-watermark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Meta & Files API
  slug: vdocipher-meta-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vdocipher Authentication
name_suffix: Authentication
oauth_flows: []
overview: VdoCipher secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VdoCipher
provider_slug: vdocipher
scheme_count: 1
schemes:
- description: 'API secret from the VdoCipher dashboard (Config tab), sent as `Authorization: Apisecret <API_SECRET>`.'
  in: header
  name: Apisecret
  parameter: Authorization
  sources:
  - openapi/vdocipher-openapi.yml
  type: apiKey
slug: vdocipher-authentication
source_filename: vdocipher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vdocipher-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Apisecret\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API secret from the VdoCipher dashboard (Config tab), sent as `Authorization:\n    Apisecret <API_SECRET>`.'\n  sources:\n  - openapi/vdocipher-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/authentication/vdocipher-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video
- Secure Video Hosting
- DRM
- Streaming
- E-Learning
- OTT
- Watermarking
---
