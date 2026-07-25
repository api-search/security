---
api_key_in: []
api_specs:
- filename: lucidworks-chunking-api-openapi.yml
  format: yaml
  label: Lucidworks Chunking API
  slug: lucidworks-chunking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-chunking-api-openapi.yml
- filename: lucidworks-classification-api-openapi.yml
  format: yaml
  label: Lucidworks Classification API
  slug: lucidworks-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-classification-api-openapi.yml
- filename: lucidworks-deployments-api-openapi.yml
  format: yaml
  label: Lucidworks Deployments API
  slug: lucidworks-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-deployments-api-openapi.yml
- filename: lucidworks-embeddings-api-openapi.yml
  format: yaml
  label: Lucidworks Embeddings API
  slug: lucidworks-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-embeddings-api-openapi.yml
- filename: lucidworks-models-api-openapi.yml
  format: yaml
  label: Lucidworks Models API
  slug: lucidworks-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-models-api-openapi.yml
- filename: lucidworks-predictions-api-openapi.yml
  format: yaml
  label: Lucidworks Predictions API
  slug: lucidworks-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-predictions-api-openapi.yml
- filename: lucidworks-queryrewrites-api-openapi.yml
  format: yaml
  label: Lucidworks QueryRewrites API
  slug: lucidworks-queryrewrites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-queryrewrites-api-openapi.yml
- filename: lucidworks-results-api-openapi.yml
  format: yaml
  label: Lucidworks Results API
  slug: lucidworks-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-results-api-openapi.yml
- filename: lucidworks-rules-api-openapi.yml
  format: yaml
  label: Lucidworks Rules API
  slug: lucidworks-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-rules-api-openapi.yml
- filename: lucidworks-signals-api-openapi.yml
  format: yaml
  label: Lucidworks Signals API
  slug: lucidworks-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-signals-api-openapi.yml
- filename: lucidworks-tokenization-api-openapi.yml
  format: yaml
  label: Lucidworks Tokenization API
  slug: lucidworks-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-tokenization-api-openapi.yml
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
