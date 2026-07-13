---
api_key_in: []
api_specs:
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Collections API
  slug: chroma-db-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Records (Embeddings) API
  slug: chroma-db-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Query and Similarity Search API
  slug: chroma-db-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Tenants and Databases API
  slug: chroma-db-tenants-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma System and Health API
  slug: chroma-db-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chroma Db Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chroma secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chroma
provider_slug: chroma-db
scheme_count: 1
schemes:
- description: Chroma Cloud API key passed in the `x-chroma-token` request header. Create the key in the Chroma Cloud dashboard; the tenant and database names for your Cloud instance are supplied alongside it. Self-hosted (open-source) Chroma servers can run with no authentication (default) or be configured with a static token (also carried in x-chroma-token, or Authorization Bearer) or HTTP basic auth by the operator. Chroma Cloud always requires a token.
  headerName: x-chroma-token
  in: header
  name: chromaToken
  sources:
  - openapi/chroma-db-openapi.yml
  - https://docs.trychroma.com/reference/chroma-api/record/query-collection
  - https://docs.trychroma.com/production/administration/auth
  type: apiKey
slug: chroma-db-authentication
source_filename: chroma-db-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/chroma-db-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: chromaToken\n  type: apiKey\n  in: header\n  headerName: x-chroma-token\n  description: >-\n    Chroma Cloud API key passed in the `x-chroma-token` request header. Create the\n    key in the Chroma Cloud dashboard; the tenant and database names for your\n    Cloud instance are supplied alongside it. Self-hosted (open-source) Chroma\n    servers can run with no authentication (default) or be configured with a\n    static token (also carried in x-chroma-token, or Authorization Bearer) or\n    HTTP basic auth by the operator. Chroma Cloud always requires a token.\n  sources:\n  - openapi/chroma-db-openapi.yml\n  - https://docs.trychroma.com/reference/chroma-api/record/query-collection\n  - https://docs.trychroma.com/production/administration/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/authentication/chroma-db-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vector Database
- Vector Index
- Vector Search
- Vector Store
- Embeddings
- Similarity Search
- RAG
- Semantic Search
- AI
- AI Inference
- Machine Learning
- Open Source
---
