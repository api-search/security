---
api_key_in: []
api_specs:
- filename: simplismart-llama-3.3-70b-openapi.yml
  format: yaml
  label: Simplismart LLM Inference API
  slug: simplismart-llm-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llama-3.3-70b-openapi.yml
- filename: simplismart-flux-dev-openapi.yml
  format: yaml
  label: Simplismart Image Generation API
  slug: simplismart-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-flux-dev-openapi.yml
- filename: simplismart-whisper-v3-openapi.yml
  format: yaml
  label: Simplismart Audio Transcription API
  slug: simplismart-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-whisper-v3-openapi.yml
- filename: simplismart-llm-training-openapi.yml
  format: yaml
  label: Simplismart Training API
  slug: simplismart-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llm-training-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Simplismart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simplismart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simplismart
provider_slug: simplismart
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token for authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/simplismart-deepseek-r1-qwen-32b-openapi.yml
  - openapi/simplismart-devstral-small-openapi.yml
  - openapi/simplismart-flux-jobs-list-openapi.yml
  - openapi/simplismart-flux-training-openapi.yml
  - openapi/simplismart-gemma3-27b-openapi.yml
  - openapi/simplismart-gemma3-4b-openapi.yml
  - openapi/simplismart-job-by-request-openapi.yml
  - openapi/simplismart-llama-3.3-70b-openapi.yml
  - openapi/simplismart-llama-4-maverick-17b-openapi.yml
  - openapi/simplismart-llama-8b-openapi.yml
  - openapi/simplismart-llm-jobs-list-openapi.yml
  - openapi/simplismart-llm-metrics-openapi.yml
  - openapi/simplismart-llm-training-openapi.yml
  - openapi/simplismart-mixtral-8x7b-openapi.yml
  - openapi/simplismart-qwen-32b-openapi.yml
  - openapi/simplismart-whisper-v2-openapi.yml
  - openapi/simplismart-whisper-v3-openapi.yml
  type: http
slug: simplismart-authentication
source_filename: simplismart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.simplismart.ai/model-suite/settings/api-keys\nnotes:\n  - Auth is a per-organisation API key passed as `Authorization: Bearer <API_KEY>` (http bearer, JWT format).\n  - Keys are created under Settings -> API Keys, carry an expiry date (or Never), and return 401 after expiry.\n  - The Python SDK/CLI use a Playground (PG) token via SIMPLISMART_PG_TOKEN for platform-management operations.\nsource: openapi/simplismart-deepseek-r1-qwen-32b-openapi.yml, openapi/simplismart-devstral-small-openapi.yml,\n  openapi/simplismart-flux-jobs-list-openapi.yml, openapi/simplismart-flux-training-openapi.yml,\n  openapi/simplismart-gemma3-27b-openapi.yml, openapi/simplismart-gemma3-4b-openapi.yml, openapi/simplismart-job-by-request-openapi.yml,\n  openapi/simplismart-llama-3.3-70b-openapi.yml, openapi/simplismart-llama-4-maverick-17b-openapi.yml,\n  openapi/simplismart-llama-8b-openapi.yml, openapi/simplismart-llm-jobs-list-openapi.yml,\
  \ openapi/simplismart-llm-metrics-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for authentication\n  sources:\n  - openapi/simplismart-deepseek-r1-qwen-32b-openapi.yml\n  - openapi/simplismart-devstral-small-openapi.yml\n  - openapi/simplismart-flux-jobs-list-openapi.yml\n  - openapi/simplismart-flux-training-openapi.yml\n  - openapi/simplismart-gemma3-27b-openapi.yml\n  - openapi/simplismart-gemma3-4b-openapi.yml\n  - openapi/simplismart-job-by-request-openapi.yml\n  - openapi/simplismart-llama-3.3-70b-openapi.yml\n  - openapi/simplismart-llama-4-maverick-17b-openapi.yml\n  - openapi/simplismart-llama-8b-openapi.yml\n  - openapi/simplismart-llm-jobs-list-openapi.yml\n  - openapi/simplismart-llm-metrics-openapi.yml\n  - openapi/simplismart-llm-training-openapi.yml\n  - openapi/simplismart-mixtral-8x7b-openapi.yml\n  - openapi/simplismart-qwen-32b-openapi.yml\n  - openapi/simplismart-whisper-v2-openapi.yml\n\
  \  - openapi/simplismart-whisper-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/authentication/simplismart-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Model Deployment
- Fine-Tuning
- MLOps
- GPU
- Speech to Text
- Image Generation
---
