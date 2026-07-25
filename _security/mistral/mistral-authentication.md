---
api_key_in: []
api_specs:
- filename: mistral-agents-api-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-agents-api-openapi.yml
- filename: mistral-audio-api-openapi.yml
  format: yaml
  label: Mistral AI Audio API
  slug: mistral-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-audio-api-openapi.yml
- filename: mistral-batch-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Batch Jobs API
  slug: mistral-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-batch-jobs-api-openapi.yml
- filename: mistral-chat-api-openapi.yml
  format: yaml
  label: Mistral AI Chat API
  slug: mistral-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-chat-api-openapi.yml
- filename: mistral-embeddings-api-openapi.yml
  format: yaml
  label: Mistral AI Embeddings API
  slug: mistral-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-embeddings-api-openapi.yml
- filename: mistral-files-api-openapi.yml
  format: yaml
  label: Mistral AI Files API
  slug: mistral-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-files-api-openapi.yml
- filename: mistral-fim-api-openapi.yml
  format: yaml
  label: Mistral AI FIM API
  slug: mistral-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fim-api-openapi.yml
- filename: mistral-fine-tuning-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning Jobs API
  slug: mistral-fine-tuning-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fine-tuning-jobs-api-openapi.yml
- filename: mistral-models-api-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-models-api-openapi.yml
- filename: mistral-moderation-api-openapi.yml
  format: yaml
  label: Mistral AI Moderation API
  slug: mistral-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-moderation-api-openapi.yml
- filename: mistral-ocr-api-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-ocr-api-openapi.yml
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
