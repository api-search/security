---
api_key_in:
- header
api_specs:
- filename: moises-music-ai-openapi.yml
  format: yaml
  label: Music AI API
  slug: music-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moises/refs/heads/main/openapi/moises-music-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moises Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moises secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moises
provider_slug: moises
scheme_count: 1
schemes:
- docs: https://music.ai/docs/api/authentication/
  format: raw key (no Bearer prefix)
  in: header
  key_management: Generate and rotate keys in the dashboard at https://music.ai/dash
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/moises-music-ai-openapi.yml
  type: apiKey
slug: moises-authentication
source_filename: moises-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://music.ai/docs/api/authentication/ , openapi/moises-music-ai-openapi.yml\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: raw key (no Bearer prefix)\n    key_management: Generate and rotate keys in the dashboard at https://music.ai/dash\n    sources: [openapi/moises-music-ai-openapi.yml]\n    docs: https://music.ai/docs/api/authentication/\nnotes: >-\n  Every request to the Music AI API must include the API key verbatim in the\n  Authorization header. There is no OAuth or OpenID Connect surface. The CLI\n  reads the key from the MUSIC_AI_API_KEY environment variable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moises/refs/heads/main/authentication/moises-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Music
- Audio
- Artificial Intelligence
- Machine Learning
- Stem Separation
- Audio Processing
- Media
- Developer Platform
- SDKs
---
