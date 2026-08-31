---
api_key_in:
- header
api_specs:
- filename: mirage-audio-api-openapi.yml
  format: yaml
  label: Mirage Audio API
  slug: mirage-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-audio-api-openapi.yml
- filename: mirage-health-api-openapi.yml
  format: yaml
  label: Mirage health API
  slug: mirage-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-health-api-openapi.yml
- filename: mirage-internal-api-openapi.yml
  format: yaml
  label: Mirage internal API
  slug: mirage-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-internal-api-openapi.yml
- filename: mirage-meta-text-overlays-api-openapi.yml
  format: yaml
  label: Mirage Meta Text Overlays API
  slug: mirage-meta-text-overlays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-meta-text-overlays-api-openapi.yml
- filename: mirage-root-api-openapi.yml
  format: yaml
  label: Mirage root API
  slug: mirage-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-root-api-openapi.yml
- filename: mirage-video-captions-api-openapi.yml
  format: yaml
  label: Mirage Video Captions API
  slug: mirage-video-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-video-captions-api-openapi.yml
- filename: mirage-videos-api-openapi.yml
  format: yaml
  label: Mirage Videos API
  slug: mirage-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/openapi/mirage-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mirage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mirage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mirage
provider_slug: mirage
scheme_count: 1
schemes:
- description: API key issued from the dashboard, sent on every request as the x-api-key header.
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://captions.ai/help/docs/api/overview
  type: apiKey
slug: mirage-authentication
source_filename: mirage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mirage-openapi-original.json\ndocs: https://captions.ai/help/docs/api/overview\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The published OpenAPI (Mirage Video API 0.0.1) declares no securitySchemes\n    object; authentication is documented in the API reference. Every request to\n    the production API must include an API key in the x-api-key header. API keys\n    are issued from the Captions/Mirage dashboard.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    API key issued from the dashboard, sent on every request as the x-api-key\n    header.\n  sources:\n  - https://captions.ai/help/docs/api/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirage/refs/heads/main/authentication/mirage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Captions
- Media
- Content Creation
- Text to Speech
- Machine-Learning
---
