---
api_key_in: []
api_specs:
- filename: mixedbread-embeddings-api-openapi.yml
  format: yaml
  label: Mixedbread Embeddings API
  slug: mixedbread-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-embeddings-api-openapi.yml
- filename: mixedbread-reranking-api-openapi.yml
  format: yaml
  label: Mixedbread Reranking API
  slug: mixedbread-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-reranking-api-openapi.yml
- filename: mixedbread-stores-api-openapi.yml
  format: yaml
  label: Mixedbread Stores API
  slug: mixedbread-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-stores-api-openapi.yml
- filename: mixedbread-parsing-api-openapi.yml
  format: yaml
  label: Mixedbread Parsing API
  slug: mixedbread-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-parsing-api-openapi.yml
- filename: mixedbread-extractions-api-openapi.yml
  format: yaml
  label: Mixedbread Extractions API
  slug: mixedbread-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-extractions-api-openapi.yml
- filename: mixedbread-files-api-openapi.yml
  format: yaml
  label: Mixedbread Files API
  slug: mixedbread-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-files-api-openapi.yml
- filename: mixedbread-completions-api-openapi.yml
  format: yaml
  label: Mixedbread Chat Completions API
  slug: mixedbread-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-completions-api-openapi.yml
- filename: mixedbread-data-sources-api-openapi.yml
  format: yaml
  label: Mixedbread Data Sources API
  slug: mixedbread-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-data-sources-api-openapi.yml
- filename: mixedbread-api-keys-api-openapi.yml
  format: yaml
  label: Mixedbread API Keys API
  slug: mixedbread-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-api-keys-api-openapi.yml
- filename: mixedbread-billing-api-openapi.yml
  format: yaml
  label: Mixedbread Billing API
  slug: mixedbread-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-billing-api-openapi.yml
- filename: mixedbread-schemas-api-openapi.yml
  format: yaml
  label: Mixedbread Schemas API
  slug: mixedbread-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-schemas-api-openapi.yml
- filename: mixedbread-admin-api-openapi.yml
  format: yaml
  label: Mixedbread Admin API
  slug: mixedbread-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-admin-api-openapi.yml
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
