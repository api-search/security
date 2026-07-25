---
api_key_in: []
api_specs:
- filename: runway-avatars-api-openapi.yml
  format: yaml
  label: Runway Avatars API
  slug: runway-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-avatars-api-openapi.yml
- filename: runway-character-performance-api-openapi.yml
  format: yaml
  label: Runway Character Performance API
  slug: runway-character-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-character-performance-api-openapi.yml
- filename: runway-documents-api-openapi.yml
  format: yaml
  label: Runway Documents API
  slug: runway-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-documents-api-openapi.yml
- filename: runway-frame-interpolation-api-openapi.yml
  format: yaml
  label: Runway Frame Interpolation API
  slug: runway-frame-interpolation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-frame-interpolation-api-openapi.yml
- filename: runway-image-to-video-api-openapi.yml
  format: yaml
  label: Runway Image to Video API
  slug: runway-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-image-to-video-api-openapi.yml
- filename: runway-lip-sync-api-openapi.yml
  format: yaml
  label: Runway Lip Sync API
  slug: runway-lip-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-lip-sync-api-openapi.yml
- filename: runway-realtime-sessions-api-openapi.yml
  format: yaml
  label: Runway Realtime Sessions API
  slug: runway-realtime-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-realtime-sessions-api-openapi.yml
- filename: runway-sound-effects-api-openapi.yml
  format: yaml
  label: Runway Sound Effects API
  slug: runway-sound-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-sound-effects-api-openapi.yml
- filename: runway-tasks-api-openapi.yml
  format: yaml
  label: Runway Tasks API
  slug: runway-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-tasks-api-openapi.yml
- filename: runway-text-to-image-api-openapi.yml
  format: yaml
  label: Runway Text to Image API
  slug: runway-text-to-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-text-to-image-api-openapi.yml
- filename: runway-text-to-video-api-openapi.yml
  format: yaml
  label: Runway Text to Video API
  slug: runway-text-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-text-to-video-api-openapi.yml
- filename: runway-uploads-api-openapi.yml
  format: yaml
  label: Runway Uploads API
  slug: runway-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-uploads-api-openapi.yml
- filename: runway-video-to-video-api-openapi.yml
  format: yaml
  label: Runway Video to Video API
  slug: runway-video-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-to-video-api-openapi.yml
- filename: runway-video-upscale-api-openapi.yml
  format: yaml
  label: Runway Video Upscale API
  slug: runway-video-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-upscale-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runway
provider_slug: runway
scheme_count: 1
schemes:
- description: API key passed via the HTTP Authorization header using the Bearer scheme. Obtain your API key from the Runway Developer Portal at https://dev.runwayml.com/.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runway-characters-openapi.yml
  - openapi/runway-image-generation-openapi.yml
  - openapi/runway-video-generation-openapi.yml
  type: http
slug: runway-authentication
source_filename: runway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runway-characters-openapi.yml, openapi/runway-image-generation-openapi.yml,\n  openapi/runway-video-generation-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed via the HTTP Authorization header using the Bearer scheme. Obtain\n    your API key from the Runway Developer Portal at https://dev.runwayml.com/.\n  sources:\n  - openapi/runway-characters-openapi.yml\n  - openapi/runway-image-generation-openapi.yml\n  - openapi/runway-video-generation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/authentication/runway-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
---
