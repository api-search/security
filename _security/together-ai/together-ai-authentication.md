---
api_key_in: []
api_specs:
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Chat Completions API
  slug: together-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Completions API
  slug: together-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Embeddings API
  slug: together-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Rerank API
  slug: together-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Images API
  slug: together-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Video API
  slug: together-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Audio API
  slug: together-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Vision API
  slug: together-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Fine-Tuning API
  slug: together-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Files API
  slug: together-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Models API
  slug: together-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Batch API
  slug: together-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Code Interpreter API
  slug: together-code-interpreter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Evaluations API
  slug: together-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Dedicated Endpoints API
  slug: together-dedicated-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Together Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Together AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Together AI
provider_slug: together-ai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/together-ai-clusters-remediation-openapi.yml
  - openapi/together-ai-openapi.yml
  - openapi/together-ai-tcloud-openapi.yml
  type: http
slug: together-ai-authentication
source_filename: together-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/together-ai-clusters-remediation-openapi.yml, openapi/together-ai-openapi.yml,\n  openapi/together-ai-tcloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/together-ai-clusters-remediation-openapi.yml\n  - openapi/together-ai-openapi.yml\n  - openapi/together-ai-tcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/authentication/together-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Foundation Models
- GPU
- Open Source AI
---
