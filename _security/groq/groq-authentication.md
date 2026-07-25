---
api_key_in: []
api_specs:
- filename: groq-audio-api-openapi.yml
  format: yaml
  label: Groq Audio API
  slug: groq-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-audio-api-openapi.yml
- filename: groq-batch-api-openapi.yml
  format: yaml
  label: Groq Batch API
  slug: groq-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-batch-api-openapi.yml
- filename: groq-chat-api-openapi.yml
  format: yaml
  label: Groq Chat API
  slug: groq-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-chat-api-openapi.yml
- filename: groq-embeddings-api-openapi.yml
  format: yaml
  label: Groq Embeddings API
  slug: groq-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-embeddings-api-openapi.yml
- filename: groq-files-api-openapi.yml
  format: yaml
  label: Groq Files API
  slug: groq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-files-api-openapi.yml
- filename: groq-fine-tuning-api-openapi.yml
  format: yaml
  label: Groq Fine Tuning API
  slug: groq-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-fine-tuning-api-openapi.yml
- filename: groq-models-api-openapi.yml
  format: yaml
  label: Groq Models API
  slug: groq-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-models-api-openapi.yml
- filename: groq-reranking-api-openapi.yml
  format: yaml
  label: Groq Reranking API
  slug: groq-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-reranking-api-openapi.yml
- filename: groq-responses-api-openapi.yml
  format: yaml
  label: Groq Responses API
  slug: groq-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-responses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Groq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Groq
provider_slug: groq
scheme_count: 1
schemes:
- bearerFormat: apiKey
  name: api_key
  scheme: bearer
  sources:
  - openapi/groq-openapi.yml
  type: http
slug: groq-authentication
source_filename: groq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/groq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  sources:\n  - openapi/groq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/authentication/groq-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- LPU
- Low Latency
---
