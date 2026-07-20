---
api_key_in: []
api_specs:
- filename: nvidia-nim-chat-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Chat Completions API
  slug: nvidia-nim-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-chat-completions-api-openapi.yml
- filename: nvidia-nim-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Completions API
  slug: nvidia-nim-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-completions-api-openapi.yml
- filename: nvidia-nim-embeddings-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Embeddings API
  slug: nvidia-nim-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-embeddings-api-openapi.yml
- filename: nvidia-nim-reranking-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Reranking API
  slug: nvidia-nim-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-reranking-api-openapi.yml
- filename: nvidia-nim-models-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Models API
  slug: nvidia-nim-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-models-api-openapi.yml
- filename: nvidia-nim-vision-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Vision Language Models API
  slug: nvidia-nim-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-vision-api-openapi.yml
- filename: nvidia-nim-health-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Health API
  slug: nvidia-nim-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-health-api-openapi.yml
- filename: nvidia-nim-image-generation-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Image Generation API
  slug: nvidia-nim-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-image-generation-api-openapi.yml
- filename: nvidia-nim-speech-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Speech API
  slug: nvidia-nim-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-speech-api-openapi.yml
- filename: nvidia-nim-biology-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Biology (BioNeMo) API
  slug: nvidia-nim-biology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-biology-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nvidia Nim Authentication
name_suffix: Authentication
oauth_flows: []
overview: NVIDIA NIM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NVIDIA NIM
provider_slug: nvidia-nim
scheme_count: 1
schemes:
- bearerFormat: nvapi-...
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nvidia-nim-biology-api-openapi.yml
  - openapi/nvidia-nim-chat-completions-api-openapi.yml
  - openapi/nvidia-nim-completions-api-openapi.yml
  - openapi/nvidia-nim-embeddings-api-openapi.yml
  - openapi/nvidia-nim-image-generation-api-openapi.yml
  - openapi/nvidia-nim-models-api-openapi.yml
  - openapi/nvidia-nim-reranking-api-openapi.yml
  - openapi/nvidia-nim-speech-api-openapi.yml
  - openapi/nvidia-nim-vision-api-openapi.yml
  type: http
slug: nvidia-nim-authentication
source_filename: nvidia-nim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/*-openapi.yml\ndocs: https://build.nvidia.com/settings\ndocs_notes: >-\n  NVIDIA developer API key (\"nvapi-...\" personal key) generated at build.nvidia.com/settings\n  and sent as `Authorization: Bearer [example key]`. The same key authenticates the hosted endpoint\n  (integrate.api.nvidia.com), NGC container pulls (nvcr.io, as the $oauthtoken password), and\n  self-hosted NIM containers (via NGC_API_KEY). No OAuth2/OIDC flow; no scopes.\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: nvapi-...\n  sources:\n  - openapi/nvidia-nim-biology-api-openapi.yml\n  - openapi/nvidia-nim-chat-completions-api-openapi.yml\n  - openapi/nvidia-nim-completions-api-openapi.yml\n  - openapi/nvidia-nim-embeddings-api-openapi.yml\n  - openapi/nvidia-nim-image-generation-api-openapi.yml\n  - openapi/nvidia-nim-models-api-openapi.yml\n  - openapi/nvidia-nim-reranking-api-openapi.yml\n\
  \  - openapi/nvidia-nim-speech-api-openapi.yml\n  - openapi/nvidia-nim-vision-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/authentication/nvidia-nim-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Inference
- Microservices
- LLM
- Foundation Models
- GPU
- Kubernetes
- NVIDIA
- OpenAI Compatible
---
