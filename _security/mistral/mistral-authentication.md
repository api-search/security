---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Mistral AI Chat API
  slug: mistral-ai-chat-api
  spec_type: OpenAPI
  url: https://docs.mistral.ai/openapi.json
- filename: mistral-embeddings-openapi.yml
  format: yaml
  label: Mistral Embeddings API
  slug: mistral-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-embeddings-openapi.yml
- filename: mistral-moderation-openapi.yml
  format: yaml
  label: Mistral Moderation API
  slug: mistral-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-moderation-openapi.yml
- filename: mistral-agents-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-agents-openapi.yml
- filename: mistral-fim-openapi.yml
  format: yaml
  label: Mistral AI FIM API
  slug: mistral-ai-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fim-openapi.yml
- filename: mistral-ocr-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-ocr-openapi.yml
- filename: mistral-fine-tuning-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning API
  slug: mistral-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fine-tuning-openapi.yml
- filename: mistral-files-openapi.yml
  format: yaml
  label: Mistral AI Files API
  slug: mistral-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-files-openapi.yml
- filename: mistral-models-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-models-openapi.yml
- filename: mistral-batch-openapi.yml
  format: yaml
  label: Mistral AI Batch API
  slug: mistral-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-batch-openapi.yml
- filename: mistral-audio-transcription-openapi.yml
  format: yaml
  label: Mistral AI Audio Transcription API
  slug: mistral-ai-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-audio-transcription-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mistral Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mistral AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mistral AI
provider_slug: mistral
scheme_count: 1
schemes:
- description: Mistral AI API key passed as a Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mistral-agents-openapi.yml
  - openapi/mistral-audio-transcription-openapi.yml
  - openapi/mistral-batch-openapi.yml
  - openapi/mistral-chat-openapi.yml
  - openapi/mistral-embeddings-openapi.yml
  - openapi/mistral-files-openapi.yml
  - openapi/mistral-fim-openapi.yml
  - openapi/mistral-fine-tuning-openapi.yml
  - openapi/mistral-models-openapi.yml
  - openapi/mistral-moderation-openapi.yml
  - openapi/mistral-ocr-openapi.yml
  type: http
slug: mistral-authentication
source_filename: mistral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mistral-agents-openapi.yml, openapi/mistral-audio-transcription-openapi.yml,\n  openapi/mistral-batch-openapi.yml, openapi/mistral-chat-openapi.yml, openapi/mistral-embeddings-openapi.yml,\n  openapi/mistral-files-openapi.yml, openapi/mistral-fim-openapi.yml, openapi/mistral-fine-tuning-openapi.yml,\n  openapi/mistral-models-openapi.yml, openapi/mistral-moderation-openapi.yml, openapi/mistral-ocr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Mistral AI API key passed as a Bearer token\n  sources:\n  - openapi/mistral-agents-openapi.yml\n  - openapi/mistral-audio-transcription-openapi.yml\n  - openapi/mistral-batch-openapi.yml\n  - openapi/mistral-chat-openapi.yml\n  - openapi/mistral-embeddings-openapi.yml\n  - openapi/mistral-files-openapi.yml\n  - openapi/mistral-fim-openapi.yml\n  - openapi/mistral-fine-tuning-openapi.yml\n  - openapi/mistral-models-openapi.yml\n\
  \  - openapi/mistral-moderation-openapi.yml\n  - openapi/mistral-ocr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/authentication/mistral-authentication.yml
summary_line: http · 1 scheme
tags: []
---
