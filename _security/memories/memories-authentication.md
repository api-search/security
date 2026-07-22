---
api_key_in:
- header
api_specs:
- filename: memories-platform-openapi.json
  format: json
  label: Memories.ai Platform API
  slug: memoriesai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/openapi/memories-platform-openapi.json
- filename: memories-stream-understanding-openapi.json
  format: json
  label: Memories.ai Stream Video Understanding API
  slug: memoriesai-stream-video-understanding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/openapi/memories-stream-understanding-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Memories Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memories secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Memories
provider_slug: memories
scheme_count: 1
schemes:
- in: header
  key_prefix: sk-mavi-
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/memories-platform-openapi.json
  - openapi/memories-stream-understanding-openapi.json
  type: apiKey
slug: memories-authentication
source_filename: memories-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/memories-platform-openapi.json, openapi/memories-stream-understanding-openapi.json\ndocs: https://api-tools.memories.ai/visual-intelligence/getting-started/create-your-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  key_prefix: sk-mavi-\n  notes: >-\n    All Memories.ai products (Visual Intelligence, Visual Search, Visual Agents,\n    Stream Understanding) authenticate with a single account-scoped API key passed\n    in the Authorization request header. Keys use the sk-mavi- prefix and are\n    created in the API Platform console (Payment -> API Key Management). One key\n    is shown once at creation. All keys on an account share the same rate-limit\n    and credit quota. No OAuth or scope surface is exposed.\n  console: https://api-platform.memories.ai/\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  key_prefix: sk-mavi-\n  sources:\n  - openapi/memories-platform-openapi.json\n\
  \  - openapi/memories-stream-understanding-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/authentication/memories-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Video Intelligence
- Video Understanding
- Video Search
- Transcription
- Embeddings
- Multimodal AI
- Content Moderation
- AI Agents
- Machine Learning
---
