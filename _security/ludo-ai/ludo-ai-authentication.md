---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ludo-ai-audio-api-openapi.yml
  format: yaml
  label: Ludo.ai Audio API
  slug: ludo-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-audio-api-openapi.yml
- filename: ludo-ai-images-api-openapi.yml
  format: yaml
  label: Ludo.ai Images API
  slug: ludo-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-images-api-openapi.yml
- filename: ludo-ai-results-api-openapi.yml
  format: yaml
  label: Ludo.ai Results API
  slug: ludo-ai-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-results-api-openapi.yml
- filename: ludo-ai-video-api-openapi.yml
  format: yaml
  label: Ludo.ai Video API
  slug: ludo-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-video-api-openapi.yml
- filename: ludo-ai-3d-models-api-openapi.yml
  format: yaml
  label: Ludo.ai 3D Models API
  slug: ludo-ai-3d-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-3d-models-api-openapi.yml
- filename: ludo-ai-account-api-openapi.yml
  format: yaml
  label: Ludo.ai Account API
  slug: ludo-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-account-api-openapi.yml
- filename: ludo-ai-animation-api-openapi.yml
  format: yaml
  label: Ludo.ai Animation API
  slug: ludo-ai-animation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-animation-api-openapi.yml
- filename: ludo-ai-authentication-api-openapi.yml
  format: yaml
  label: Ludo.ai Authentication API
  slug: ludo-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-authentication-api-openapi.yml
- filename: ludo-ai-documentation-api-openapi.yml
  format: yaml
  label: Ludo.ai Documentation API
  slug: ludo-ai-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-documentation-api-openapi.yml
- filename: ludo-ai-files-api-openapi.yml
  format: yaml
  label: Ludo.ai Files API
  slug: ludo-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-files-api-openapi.yml
- filename: ludo-ai-generations-api-openapi.yml
  format: yaml
  label: Ludo.ai Generations API
  slug: ludo-ai-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-generations-api-openapi.yml
- filename: ludo-ai-jobs-api-openapi.yml
  format: yaml
  label: Ludo.ai Jobs API
  slug: ludo-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-jobs-api-openapi.yml
- filename: ludo-ai-spritesheets-api-openapi.yml
  format: yaml
  label: Ludo.ai Spritesheets API
  slug: ludo-ai-spritesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-spritesheets-api-openapi.yml
- filename: ludo-ai-videos-api-openapi.yml
  format: yaml
  label: Ludo.ai Videos API
  slug: ludo-ai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ludo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ludo.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ludo.ai
provider_slug: ludo-ai
scheme_count: 1
schemes:
- description: 'API key authentication. Pass your API key in the Authentication header with the format: ApiKey YOUR_API_KEY'
  in: header
  name: apiKeyAuth
  parameter: Authentication
  sources:
  - openapi/ludo-ai-rest-api-openapi.yml
  type: apiKey
slug: ludo-ai-authentication
source_filename: ludo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ludo-ai-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: 'API key authentication. Pass your API key in the Authentication header with\n    the format: ApiKey YOUR_API_KEY'\n  sources:\n  - openapi/ludo-ai-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/authentication/ludo-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Asset Generation
- Game Design
- Game Development
- Game Asset Generation
- AI Art
- Sprite Sheets
---
