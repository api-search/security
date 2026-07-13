---
api_key_in: []
api_specs:
- filename: hailuo-ai-openapi.yml
  format: yaml
  label: Hailuo Video Generation API
  slug: hailuo-ai-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/openapi/hailuo-ai-openapi.yml
- filename: hailuo-ai-openapi.yml
  format: yaml
  label: MiniMax Text-to-Speech (T2A) API
  slug: hailuo-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/openapi/hailuo-ai-openapi.yml
- filename: hailuo-ai-openapi.yml
  format: yaml
  label: MiniMax Chat Completions API
  slug: hailuo-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/openapi/hailuo-ai-openapi.yml
- filename: hailuo-ai-openapi.yml
  format: yaml
  label: MiniMax Music Generation API
  slug: hailuo-ai-music-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/openapi/hailuo-ai-openapi.yml
- filename: hailuo-ai-openapi.yml
  format: yaml
  label: MiniMax Files API
  slug: hailuo-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/openapi/hailuo-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hailuo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hailuo AI / MiniMax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hailuo AI / MiniMax
provider_slug: hailuo-ai
scheme_count: 1
schemes:
- description: 'Bearer API key created in the MiniMax platform console under Account Management > API Keys (both pay-as-you-go and subscription keys are supported). Passed as `Authorization: Bearer {api_key}` on every HTTP request and on the T2A WebSocket handshake.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hailuo-ai-openapi.yml
  - https://platform.minimax.io/docs/api-reference/speech-t2a-http
  type: http
slug: hailuo-ai-authentication
source_filename: hailuo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hailuo-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key created in the MiniMax platform console under Account\n    Management > API Keys (both pay-as-you-go and subscription keys are supported).\n    Passed as `Authorization: Bearer {api_key}` on every HTTP request and on the\n    T2A WebSocket handshake.'\n  sources:\n  - openapi/hailuo-ai-openapi.yml\n  - https://platform.minimax.io/docs/api-reference/speech-t2a-http\nnotes: >-\n  International users authenticate against api.minimax.io / intl.minimaxi.com;\n  mainland China users authenticate against api.minimaxi.chat. The same Bearer\n  scheme applies to video generation, chat completions, text-to-speech, and music\n  generation endpoints, and to the real-time T2A WebSocket.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hailuo-ai/refs/heads/main/authentication/hailuo-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- Text to Speech
- LLM
- Foundation Models
---
