---
api_key_in: []
api_specs:
- filename: lucidworks-ai-platform-openapi.yml
  format: yaml
  label: Lucidworks AI Platform API
  slug: ai-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-ai-platform-openapi.yml
- filename: lucidworks-embeddings-openapi.yml
  format: yaml
  label: Lucidworks Embeddings and Classification API
  slug: embeddings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-embeddings-openapi.yml
- filename: lucidworks-signals-openapi.yml
  format: yaml
  label: Lucidworks Signals API
  slug: signals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-signals-openapi.yml
- filename: lucidworks-rules-openapi.yml
  format: yaml
  label: Lucidworks Rules and Query Rewrites API
  slug: rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-rules-openapi.yml
- filename: lucidworks-chunking-openapi.yml
  format: yaml
  label: Lucidworks Content Chunking API
  slug: chunking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-chunking-openapi.yml
- filename: lucidworks-models-openapi.yml
  format: yaml
  label: Lucidworks Model Management API
  slug: models
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-models-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lucidworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucidworks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lucidworks
provider_slug: lucidworks
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lucidworks-ai-platform-openapi.yml
  - openapi/lucidworks-chunking-openapi.yml
  - openapi/lucidworks-embeddings-openapi.yml
  - openapi/lucidworks-models-openapi.yml
  - openapi/lucidworks-rules-openapi.yml
  - openapi/lucidworks-signals-openapi.yml
  type: http
slug: lucidworks-authentication
source_filename: lucidworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lucidworks-ai-platform-openapi.yml, openapi/lucidworks-chunking-openapi.yml,\n  openapi/lucidworks-embeddings-openapi.yml, openapi/lucidworks-models-openapi.yml, openapi/lucidworks-rules-openapi.yml,\n  openapi/lucidworks-signals-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lucidworks-ai-platform-openapi.yml\n  - openapi/lucidworks-chunking-openapi.yml\n  - openapi/lucidworks-embeddings-openapi.yml\n  - openapi/lucidworks-models-openapi.yml\n  - openapi/lucidworks-rules-openapi.yml\n  - openapi/lucidworks-signals-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/authentication/lucidworks-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Artificial Intelligence
- Enterprise Search
- Vector Search
- RAG
- Commerce
---
