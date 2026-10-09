---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: octen-ai-answer-api-openapi.yml
  format: yaml
  label: Octen Answer API
  slug: octen-ai-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-answer-api-openapi.yml
- filename: octen-ai-broad-search-api-openapi.yml
  format: yaml
  label: Octen Broad Search API
  slug: octen-ai-broad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-broad-search-api-openapi.yml
- filename: octen-ai-business-search-api-openapi.yml
  format: yaml
  label: Octen Business Search API
  slug: octen-ai-business-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-business-search-api-openapi.yml
- filename: octen-ai-embedding-api-openapi.yml
  format: yaml
  label: Octen Embedding API
  slug: octen-ai-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-embedding-api-openapi.yml
- filename: octen-ai-extract-api-openapi.yml
  format: yaml
  label: Octen Extract API
  slug: octen-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-extract-api-openapi.yml
- filename: octen-ai-grounded-generation-api-openapi.yml
  format: yaml
  label: Octen Grounded Generation API
  slug: octen-ai-grounded-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-grounded-generation-api-openapi.yml
- filename: octen-ai-image-search-api-openapi.yml
  format: yaml
  label: Octen Image Search API
  slug: octen-ai-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-image-search-api-openapi.yml
- filename: octen-ai-images-api-openapi.yml
  format: yaml
  label: Octen Images API
  slug: octen-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-images-api-openapi.yml
- filename: octen-ai-messages-api-openapi.yml
  format: yaml
  label: Octen Messages API
  slug: octen-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-messages-api-openapi.yml
- filename: octen-ai-news-search-api-openapi.yml
  format: yaml
  label: Octen News Search API
  slug: octen-ai-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-news-search-api-openapi.yml
- filename: octen-ai-research-api-openapi.yml
  format: yaml
  label: Octen Research API
  slug: octen-ai-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-research-api-openapi.yml
- filename: octen-ai-search-api-openapi.yml
  format: yaml
  label: Octen Search API
  slug: octen-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-search-api-openapi.yml
- filename: octen-ai-video-search-api-openapi.yml
  format: yaml
  label: Octen Video Search API
  slug: octen-ai-video-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-video-search-api-openapi.yml
- filename: octen-ai-videos-api-openapi.yml
  format: yaml
  label: Octen Videos API
  slug: octen-ai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-videos-api-openapi.yml
- filename: octen-ai-vl-embedding-api-openapi.yml
  format: yaml
  label: Octen Vl Embedding API
  slug: octen-ai-vl-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-vl-embedding-api-openapi.yml
- filename: octen-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Octen Chat Completions API
  slug: octen-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-chat-completions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Octen Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octen secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Octen
provider_slug: octen-ai
scheme_count: 2
schemes:
- description: 'Bearer token used for request authentication. Alternatively, you can send the API key in the `x-api-key` header. Note: A payment method is required to use the API.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/octen-ai-openapi.yml
  type: http
- description: 'API key used for request authentication. Alternatively, you can send the key as a Bearer token in the `Authorization` header. Note: A payment method is required to use the API.'
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/octen-ai-openapi.yml
  type: apiKey
slug: octen-ai-authentication
source_filename: octen-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: 'openapi/octen-ai-openapi.yml; https://docs.octen.ai/overview/quickstart.md (x-api-key header example); OpenAPI securitySchemes: bearerAuth + apiKeyAuth, payment method required'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token used for request authentication. Alternatively, you can send the API key in the `x-api-key` header. Note: A payment method is required to use the API.'\n  sources:\n  - openapi/octen-ai-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'API key used for request authentication. Alternatively, you can send the key as a Bearer token in the `Authorization` header. Note: A payment method is required to use the API.'\n  sources:\n  - openapi/octen-ai-openapi.yml\ndocs: https://docs.octen.ai/overview/quickstart\nkey_management: https://octen.ai/platform/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/authentication/octen-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Search
- Web Search
- AI
- LLM
- Embeddings
- Content Extraction
- Model Gateway
- MCP
- Agents
- Deep Research
- Company
---
