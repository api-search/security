---
api_key_in: []
api_specs:
- filename: xai-openapi.json
  format: json
  label: xAI Chat Completions API
  slug: xai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Responses API
  slug: xai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Images API
  slug: xai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Video Generation API
  slug: xai-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Voice API
  slug: xai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Embeddings API
  slug: xai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Models API
  slug: xai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Batch API
  slug: xai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xai Authentication
name_suffix: Authentication
oauth_flows: []
overview: xAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: xAI
provider_slug: xai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xai-openapi.json
  type: http
slug: xai-authentication
source_filename: xai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/xai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/authentication/xai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Foundation Models
- Grok
- Generative AI
---
