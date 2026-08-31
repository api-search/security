---
api_key_in:
- header
api_specs:
- filename: heygen-account-api-openapi.yml
  format: yaml
  label: HeyGen Account API
  slug: heygen-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-account-api-openapi.yml
- filename: heygen-assets-api-openapi.yml
  format: yaml
  label: HeyGen Assets API
  slug: heygen-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-assets-api-openapi.yml
- filename: heygen-avatars-api-openapi.yml
  format: yaml
  label: HeyGen Avatars API
  slug: heygen-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-avatars-api-openapi.yml
- filename: heygen-digital-twins-api-openapi.yml
  format: yaml
  label: HeyGen Digital Twins API
  slug: heygen-digital-twins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-digital-twins-api-openapi.yml
- filename: heygen-folders-api-openapi.yml
  format: yaml
  label: HeyGen Folders API
  slug: heygen-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-folders-api-openapi.yml
- filename: heygen-photo-avatars-api-openapi.yml
  format: yaml
  label: HeyGen Photo Avatars API
  slug: heygen-photo-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-photo-avatars-api-openapi.yml
- filename: heygen-streaming-api-openapi.yml
  format: yaml
  label: HeyGen Streaming API
  slug: heygen-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-streaming-api-openapi.yml
- filename: heygen-templates-api-openapi.yml
  format: yaml
  label: HeyGen Templates API
  slug: heygen-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-templates-api-openapi.yml
- filename: heygen-video-translation-api-openapi.yml
  format: yaml
  label: HeyGen Video Translation API
  slug: heygen-video-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-video-translation-api-openapi.yml
- filename: heygen-videos-api-openapi.yml
  format: yaml
  label: HeyGen Videos API
  slug: heygen-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-videos-api-openapi.yml
- filename: heygen-voices-api-openapi.yml
  format: yaml
  label: HeyGen Voices API
  slug: heygen-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-voices-api-openapi.yml
- filename: heygen-webhooks-api-openapi.yml
  format: yaml
  label: HeyGen Webhooks API
  slug: heygen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Heygen Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeyGen secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HeyGen
provider_slug: heygen
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/heygen-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/heygen-openapi.yml
  type: apiKey
slug: heygen-authentication
source_filename: heygen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heygen-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/heygen-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/heygen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/authentication/heygen-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Generative AI
- Video
- Avatars
- Voice Cloning
- Text-to-Speech
- Lipsync
- Translation
- Streaming
- MCP
---
