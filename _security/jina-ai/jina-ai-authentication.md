---
api_key_in: []
api_specs:
- filename: jina-ai-embeddings-openapi.yml
  format: yaml
  label: Jina AI Embeddings API
  slug: embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-embeddings-openapi.yml
- filename: jina-ai-reader-openapi.yml
  format: yaml
  label: Jina AI Reader API
  slug: reader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-reader-openapi.yml
- filename: jina-ai-reranker-openapi.yml
  format: yaml
  label: Jina AI Reranker API
  slug: reranker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-reranker-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jina Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jina AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jina AI
provider_slug: jina-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/jina-ai-embeddings-openapi.yml
  - openapi/jina-ai-reader-openapi.yml
  - openapi/jina-ai-reranker-openapi.yml
  type: http
slug: jina-ai-authentication
source_filename: jina-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jina-ai-embeddings-openapi.yml, openapi/jina-ai-reader-openapi.yml, openapi/jina-ai-reranker-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/jina-ai-embeddings-openapi.yml\n  - openapi/jina-ai-reader-openapi.yml\n  - openapi/jina-ai-reranker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/authentication/jina-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Embeddings
- Machine Learning
- Reranking
- Search
---
