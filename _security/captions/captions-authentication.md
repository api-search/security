---
api_key_in:
- header
api_specs:
- filename: captions-audio-api-openapi.yml
  format: yaml
  label: Captions Audio API
  slug: captions-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-audio-api-openapi.yml
- filename: captions-health-api-openapi.yml
  format: yaml
  label: Captions health API
  slug: captions-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-health-api-openapi.yml
- filename: captions-internal-api-openapi.yml
  format: yaml
  label: Captions internal API
  slug: captions-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-internal-api-openapi.yml
- filename: captions-meta-text-overlays-api-openapi.yml
  format: yaml
  label: Captions Meta Text Overlays API
  slug: captions-meta-text-overlays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-meta-text-overlays-api-openapi.yml
- filename: captions-root-api-openapi.yml
  format: yaml
  label: Captions root API
  slug: captions-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-root-api-openapi.yml
- filename: captions-video-captions-api-openapi.yml
  format: yaml
  label: Captions Video Captions API
  slug: captions-video-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-video-captions-api-openapi.yml
- filename: captions-videos-api-openapi.yml
  format: yaml
  label: Captions Videos API
  slug: captions-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Captions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Captions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Captions
provider_slug: captions
scheme_count: 1
schemes:
- description: API key issued from the Mirage platform dashboard. Sent on every request as the `x-api-key` request header.
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://captions.ai/help/docs/api/overview
  type: apiKey
slug: captions-authentication
source_filename: captions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://captions.ai/help/docs/api/overview\ndocs: https://captions.ai/help/docs/api/overview\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Every request to the Mirage Video API must include an `x-api-key` header\n    containing an API key. Keys are minted in the Mirage platform dashboard at\n    https://platform.mirage.app/. The published OpenAPI does not formally\n    declare a securityScheme; the auth model is documented on the API overview\n    page. No OAuth, no scopes.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    API key issued from the Mirage platform dashboard. Sent on every request as\n    the `x-api-key` request header.\n  sources:\n  - https://captions.ai/help/docs/api/overview\nkey_management:\n  dashboard: https://platform.mirage.app/\n  provisioning: Generate and revoke keys in the Mirage platform dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/authentication/captions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Video
- Artificial Intelligence
- Video Editing
- Video Generation
- Captions
- Subtitles
- Text-to-Speech
- AI Avatars
- Content Creation
- Media
---
