---
api_key_in: []
api_specs:
- filename: mistral-ai-chat-completions-openapi.yml
  format: yaml
  label: Mistral AI Chat Completions API
  slug: chat-completions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-chat-completions-openapi.yml
- filename: mistral-ai-embeddings-openapi.yml
  format: yaml
  label: Mistral AI Embeddings API
  slug: embeddings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-embeddings-openapi.yml
- filename: mistral-ai-agents-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-agents-openapi.yml
- filename: mistral-ai-fine-tuning-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning API
  slug: fine-tuning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-fine-tuning-openapi.yml
- filename: mistral-ai-ocr-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: ocr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-ocr-openapi.yml
- filename: mistral-ai-models-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: models
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-models-openapi.yml
- filename: mistral-ai-forge-openapi.yml
  format: yaml
  label: Mistral AI Forge API
  slug: forge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-forge-openapi.yml
- filename: mistral-ai-batch-openapi.yml
  format: yaml
  label: Mistral AI Batch API
  slug: batch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-batch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mistral Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mistral AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mistral AI
provider_slug: mistral-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mistral-ai-agents-openapi.yml
  - openapi/mistral-ai-batch-openapi.yml
  - openapi/mistral-ai-chat-completions-openapi.yml
  - openapi/mistral-ai-embeddings-openapi.yml
  - openapi/mistral-ai-fine-tuning-openapi.yml
  - openapi/mistral-ai-forge-openapi.yml
  - openapi/mistral-ai-models-openapi.yml
  - openapi/mistral-ai-ocr-openapi.yml
  type: http
slug: mistral-ai-authentication
source_filename: mistral-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mistral-ai-agents-openapi.yml, openapi/mistral-ai-batch-openapi.yml, openapi/mistral-ai-chat-completions-openapi.yml,\n  openapi/mistral-ai-embeddings-openapi.yml, openapi/mistral-ai-fine-tuning-openapi.yml, openapi/mistral-ai-forge-openapi.yml,\n  openapi/mistral-ai-models-openapi.yml, openapi/mistral-ai-ocr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/mistral-ai-agents-openapi.yml\n  - openapi/mistral-ai-batch-openapi.yml\n  - openapi/mistral-ai-chat-completions-openapi.yml\n  - openapi/mistral-ai-embeddings-openapi.yml\n  - openapi/mistral-ai-fine-tuning-openapi.yml\n  - openapi/mistral-ai-forge-openapi.yml\n  - openapi/mistral-ai-models-openapi.yml\n  - openapi/mistral-ai-ocr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/authentication/mistral-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
---
