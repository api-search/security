---
api_key_in: []
api_specs:
- filename: minimax-ai-files-api-openapi.yml
  format: yaml
  label: MiniMax Files API
  slug: minimax-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-files-api-openapi.yml
- filename: minimax-ai-image-api-openapi.yml
  format: yaml
  label: MiniMax Image API
  slug: minimax-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-image-api-openapi.yml
- filename: minimax-ai-music-api-openapi.yml
  format: yaml
  label: MiniMax Music API
  slug: minimax-ai-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-music-api-openapi.yml
- filename: minimax-ai-text-generation-api-openapi.yml
  format: yaml
  label: MiniMax Text Generation API
  slug: minimax-ai-text-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-text-generation-api-openapi.yml
- filename: minimax-ai-text-to-audio-api-openapi.yml
  format: yaml
  label: MiniMax Text to Audio API
  slug: minimax-ai-text-to-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-text-to-audio-api-openapi.yml
- filename: minimax-ai-video-api-openapi.yml
  format: yaml
  label: MiniMax Video API
  slug: minimax-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-video-api-openapi.yml
- filename: minimax-ai-voice-api-openapi.yml
  format: yaml
  label: MiniMax Voice API
  slug: minimax-ai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-voice-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Minimax Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MiniMax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MiniMax
provider_slug: minimax-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/minimax-ai-openapi.json
  type: http
slug: minimax-ai-authentication
source_filename: minimax-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/minimax-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/minimax-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/authentication/minimax-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Inference
- Multimodal
- Voice
- Video
- Music
- Image
---
