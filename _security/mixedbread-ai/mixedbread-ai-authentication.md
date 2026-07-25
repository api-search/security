---
api_key_in: []
api_specs:
- filename: mixedbread-ai-admin-api-openapi.yml
  format: yaml
  label: Mixedbread admin API
  slug: mixedbread-ai-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-admin-api-openapi.yml
- filename: mixedbread-ai-api-keys-api-openapi.yml
  format: yaml
  label: Mixedbread api_keys API
  slug: mixedbread-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-api-keys-api-openapi.yml
- filename: mixedbread-ai-billing-api-openapi.yml
  format: yaml
  label: Mixedbread billing API
  slug: mixedbread-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-billing-api-openapi.yml
- filename: mixedbread-ai-completions-api-openapi.yml
  format: yaml
  label: Mixedbread completions API
  slug: mixedbread-ai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-completions-api-openapi.yml
- filename: mixedbread-ai-data-sources-api-openapi.yml
  format: yaml
  label: Mixedbread data_sources API
  slug: mixedbread-ai-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-data-sources-api-openapi.yml
- filename: mixedbread-ai-deprecated-vector-stores-api-openapi.yml
  format: yaml
  label: Mixedbread deprecated_vector_stores API
  slug: mixedbread-ai-deprecated-vector-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-deprecated-vector-stores-api-openapi.yml
- filename: mixedbread-ai-embeddings-api-openapi.yml
  format: yaml
  label: Mixedbread Embeddings API
  slug: mixedbread-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-embeddings-api-openapi.yml
- filename: mixedbread-ai-extractions-api-openapi.yml
  format: yaml
  label: Mixedbread extractions API
  slug: mixedbread-ai-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-extractions-api-openapi.yml
- filename: mixedbread-ai-files-api-openapi.yml
  format: yaml
  label: Mixedbread files API
  slug: mixedbread-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-files-api-openapi.yml
- filename: mixedbread-ai-mixedbread-embeddings-api-api-openapi.yml
  format: yaml
  label: Mixedbread Mixedbread Embeddings API API
  slug: mixedbread-ai-mixedbread-embeddings-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-mixedbread-embeddings-api-api-openapi.yml
- filename: mixedbread-ai-parsing-api-openapi.yml
  format: yaml
  label: Mixedbread parsing API
  slug: mixedbread-ai-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-parsing-api-openapi.yml
- filename: mixedbread-ai-reranking-api-openapi.yml
  format: yaml
  label: Mixedbread Reranking API
  slug: mixedbread-ai-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-reranking-api-openapi.yml
- filename: mixedbread-ai-schemas-api-openapi.yml
  format: yaml
  label: Mixedbread schemas API
  slug: mixedbread-ai-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-schemas-api-openapi.yml
- filename: mixedbread-ai-stores-api-openapi.yml
  format: yaml
  label: Mixedbread stores API
  slug: mixedbread-ai-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mixedbread Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mixedbread secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mixedbread
provider_slug: mixedbread-ai
scheme_count: 1
schemes:
- description: Api key to access Mixedbreads API
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/mixedbread-admin-api-openapi.yml
  - openapi/mixedbread-api-keys-api-openapi.yml
  - openapi/mixedbread-billing-api-openapi.yml
  - openapi/mixedbread-completions-api-openapi.yml
  - openapi/mixedbread-data-sources-api-openapi.yml
  - openapi/mixedbread-embeddings-api-openapi.yml
  - openapi/mixedbread-extractions-api-openapi.yml
  - openapi/mixedbread-files-api-openapi.yml
  - openapi/mixedbread-parsing-api-openapi.yml
  - openapi/mixedbread-reranking-api-openapi.yml
  - openapi/mixedbread-schemas-api-openapi.yml
  - openapi/mixedbread-stores-api-openapi.yml
  type: http
slug: mixedbread-ai-authentication
source_filename: mixedbread-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mixedbread-admin-api-openapi.yml, openapi/mixedbread-api-keys-api-openapi.yml,\n  openapi/mixedbread-billing-api-openapi.yml, openapi/mixedbread-completions-api-openapi.yml,\n  openapi/mixedbread-data-sources-api-openapi.yml, openapi/mixedbread-embeddings-api-openapi.yml,\n  openapi/mixedbread-extractions-api-openapi.yml, openapi/mixedbread-files-api-openapi.yml,\n  openapi/mixedbread-parsing-api-openapi.yml, openapi/mixedbread-reranking-api-openapi.yml,\n  openapi/mixedbread-schemas-api-openapi.yml, openapi/mixedbread-stores-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: Api key to access Mixedbreads API\n  sources:\n  - openapi/mixedbread-admin-api-openapi.yml\n  - openapi/mixedbread-api-keys-api-openapi.yml\n  - openapi/mixedbread-billing-api-openapi.yml\n  - openapi/mixedbread-completions-api-openapi.yml\n  - openapi/mixedbread-data-sources-api-openapi.yml\n\
  \  - openapi/mixedbread-embeddings-api-openapi.yml\n  - openapi/mixedbread-extractions-api-openapi.yml\n  - openapi/mixedbread-files-api-openapi.yml\n  - openapi/mixedbread-parsing-api-openapi.yml\n  - openapi/mixedbread-reranking-api-openapi.yml\n  - openapi/mixedbread-schemas-api-openapi.yml\n  - openapi/mixedbread-stores-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/authentication/mixedbread-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Embeddings
- Reranking
- Search
- Retrieval
- RAG
- Vector Database
- Multimodal
- Parsing
- Open Weights
---
