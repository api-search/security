---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jina-ai-reader-api-openapi.yml
  format: yaml
  label: Jina AI Reader API
  slug: jina-ai-reader-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-reader-api-openapi.yml
- filename: jina-ai-batch-embeddings-api-openapi.yml
  format: yaml
  label: Jina AI Batch Embeddings API
  slug: jina-ai-batch-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-batch-embeddings-api-openapi.yml
- filename: jina-ai-generative-models-api-openapi.yml
  format: yaml
  label: Jina AI Generative Models API
  slug: jina-ai-generative-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-generative-models-api-openapi.yml
- filename: jina-ai-model-list-api-openapi.yml
  format: yaml
  label: Jina AI Model List API
  slug: jina-ai-model-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-model-list-api-openapi.yml
- filename: jina-ai-search-api-openapi.yml
  format: yaml
  label: Jina AI Search API
  slug: jina-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-search-api-openapi.yml
- filename: jina-ai-search-foundation-models-api-openapi.yml
  format: yaml
  label: Jina AI Search Foundation Models API
  slug: jina-ai-search-foundation-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jina-ai/openapi/jina-ai-search-foundation-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Jina AI Authentication
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
source_yaml_url: https://artifacts.apis.io/jina-ai/authentication/jina-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Embeddings
- Machine Learning
- Reranking
- Search
---
