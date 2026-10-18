---
anonymous_access: false
api_key_in: []
api_specs:
- filename: llmgateway-io-audio-api-openapi.yml
  format: yaml
  label: LLM Gateway Audio API
  slug: llmgateway-io-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-audio-api-openapi.yml
- filename: llmgateway-io-decisions-api-openapi.yml
  format: yaml
  label: LLM Gateway Decisions API
  slug: llmgateway-io-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-decisions-api-openapi.yml
- filename: llmgateway-io-embeddings-api-openapi.yml
  format: yaml
  label: LLM Gateway Embeddings API
  slug: llmgateway-io-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-embeddings-api-openapi.yml
- filename: llmgateway-io-images-api-openapi.yml
  format: yaml
  label: LLM Gateway Images API
  slug: llmgateway-io-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-images-api-openapi.yml
- filename: llmgateway-io-key-api-openapi.yml
  format: yaml
  label: LLM Gateway Key API
  slug: llmgateway-io-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-key-api-openapi.yml
- filename: llmgateway-io-llm-gateway-api-api-openapi.yml
  format: yaml
  label: LLM Gateway LLM Gateway API
  slug: llmgateway-io-llm-gateway-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-llm-gateway-api-api-openapi.yml
- filename: llmgateway-io-messages-api-openapi.yml
  format: yaml
  label: LLM Gateway Messages API
  slug: llmgateway-io-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-messages-api-openapi.yml
- filename: llmgateway-io-models-api-openapi.yml
  format: yaml
  label: LLM Gateway Models API
  slug: llmgateway-io-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-models-api-openapi.yml
- filename: llmgateway-io-moderations-api-openapi.yml
  format: yaml
  label: LLM Gateway Moderations API
  slug: llmgateway-io-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-moderations-api-openapi.yml
- filename: llmgateway-io-ocr-api-openapi.yml
  format: yaml
  label: LLM Gateway Ocr API
  slug: llmgateway-io-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-ocr-api-openapi.yml
- filename: llmgateway-io-realtime-api-openapi.yml
  format: yaml
  label: LLM Gateway Realtime API
  slug: llmgateway-io-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-realtime-api-openapi.yml
- filename: llmgateway-io-rerank-api-openapi.yml
  format: yaml
  label: LLM Gateway Rerank API
  slug: llmgateway-io-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-rerank-api-openapi.yml
- filename: llmgateway-io-search-api-openapi.yml
  format: yaml
  label: LLM Gateway Search API
  slug: llmgateway-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-search-api-openapi.yml
- filename: llmgateway-io-systemone-api-openapi.yml
  format: yaml
  label: LLM Gateway Systemone API
  slug: llmgateway-io-systemone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-systemone-api-openapi.yml
- filename: llmgateway-io-videos-api-openapi.yml
  format: yaml
  label: LLM Gateway Videos API
  slug: llmgateway-io-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-videos-api-openapi.yml
- filename: llmgateway-io-chat-completions-api-openapi.yml
  format: yaml
  label: LLM Gateway Chat Completions API
  slug: llmgateway-io-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Llmgateway Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: LLM Gateway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LLM Gateway
provider_slug: llmgateway-io
scheme_count: 1
schemes:
- description: Bearer token authentication using API keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/llmgateway-io-gateway-api-openapi.yml
  type: http
slug: llmgateway-io-authentication
source_filename: llmgateway-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/llmgateway-io-gateway-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using API keys\n  sources:\n  - openapi/llmgateway-io-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/authentication/llmgateway-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM Gateway
- Decision Support
- Structured Outputs
- Inference
- MCP
---
