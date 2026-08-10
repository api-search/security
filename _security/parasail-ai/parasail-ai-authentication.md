---
api_key_in: []
api_specs:
- filename: parasail-ai-batch-api-openapi.yml
  format: yaml
  label: Parasail Batch API
  slug: parasail-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-batch-api-openapi.yml
- filename: parasail-ai-chat-api-openapi.yml
  format: yaml
  label: Parasail Chat API
  slug: parasail-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-chat-api-openapi.yml
- filename: parasail-ai-completions-api-openapi.yml
  format: yaml
  label: Parasail Completions API
  slug: parasail-ai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-completions-api-openapi.yml
- filename: parasail-ai-deployments-api-openapi.yml
  format: yaml
  label: Parasail Deployments API
  slug: parasail-ai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-deployments-api-openapi.yml
- filename: parasail-ai-embeddings-api-openapi.yml
  format: yaml
  label: Parasail Embeddings API
  slug: parasail-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-embeddings-api-openapi.yml
- filename: parasail-ai-files-api-openapi.yml
  format: yaml
  label: Parasail Files API
  slug: parasail-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-files-api-openapi.yml
- filename: parasail-ai-models-api-openapi.yml
  format: yaml
  label: Parasail Models API
  slug: parasail-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/openapi/parasail-ai-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Parasail Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parasail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parasail
provider_slug: parasail-ai
scheme_count: 1
schemes:
- description: Send your Parasail API key as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parasail-batch-api-openapi.yml
  - openapi/parasail-dedicated-api-openapi.yml
  - openapi/parasail-inference-api-openapi.yml
  type: http
slug: parasail-ai-authentication
source_filename: parasail-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parasail-batch-api-openapi.yml, openapi/parasail-dedicated-api-openapi.yml,\n  openapi/parasail-inference-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Send your Parasail API key as a Bearer token.\n  sources:\n  - openapi/parasail-batch-api-openapi.yml\n  - openapi/parasail-dedicated-api-openapi.yml\n  - openapi/parasail-inference-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parasail-ai/refs/heads/main/authentication/parasail-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- GPU
- Inference
- Large Language Models
- Open Source Models
- Hugging Face
- Batch
- Embeddings
- Tokenmaxxing
- Supercloud
---
