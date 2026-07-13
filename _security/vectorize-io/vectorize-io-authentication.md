---
api_key_in: []
api_specs:
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Pipelines API
  slug: vectorize-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Retrieval API
  slug: vectorize-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Connectors API
  slug: vectorize-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize File Upload API
  slug: vectorize-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Extraction (Iris) API
  slug: vectorize-extraction-iris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Deep Research API
  slug: vectorize-deep-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vectorize Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vectorize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vectorize
provider_slug: vectorize-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Vectorize API access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vectorize-io-openapi.yml
  type: http
slug: vectorize-io-authentication
source_filename: vectorize-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vectorize-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Vectorize API access token passed as a Bearer token.\n  sources:\n  - openapi/vectorize-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/authentication/vectorize-io-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- RAG
- Vectorization
- Embeddings
- Retrieval
- Vector Database
---
