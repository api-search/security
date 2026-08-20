---
api_key_in: []
api_specs:
- filename: rightnow-audio-api-openapi.yml
  format: yaml
  label: RightNow AI Audio API
  slug: rightnow-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-audio-api-openapi.yml
- filename: rightnow-chat-api-openapi.yml
  format: yaml
  label: RightNow AI Chat API
  slug: rightnow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-chat-api-openapi.yml
- filename: rightnow-embeddings-api-openapi.yml
  format: yaml
  label: RightNow AI Embeddings API
  slug: rightnow-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-embeddings-api-openapi.yml
- filename: rightnow-images-api-openapi.yml
  format: yaml
  label: RightNow AI Images API
  slug: rightnow-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-images-api-openapi.yml
- filename: rightnow-models-api-openapi.yml
  format: yaml
  label: RightNow AI Models API
  slug: rightnow-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-models-api-openapi.yml
- filename: rightnow-rerank-api-openapi.yml
  format: yaml
  label: RightNow AI Rerank API
  slug: rightnow-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-rerank-api-openapi.yml
- filename: rightnow-responses-api-openapi.yml
  format: yaml
  label: RightNow AI Responses API
  slug: rightnow-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-responses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rightnow Authentication
name_suffix: Authentication
oauth_flows: []
overview: RightNow AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RightNow AI
provider_slug: rightnow
scheme_count: 1
schemes:
- description: RunInfra API key. Generate at https://runinfra.ai/settings/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rightnow-openapi.json
  type: http
slug: rightnow-authentication
source_filename: rightnow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rightnow-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: RunInfra API key. Generate at https://runinfra.ai/settings/api-keys\n  sources:\n  - openapi/rightnow-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/authentication/rightnow-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- LLM Inference
- GPU
- Model Deployment
- Serverless
- OpenAI-Compatible
- Embeddings
- MLOps
---
