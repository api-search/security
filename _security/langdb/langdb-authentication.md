---
api_key_in: []
api_specs:
- filename: langdb-analytics-api-openapi.yml
  format: yaml
  label: LangDB Analytics API
  slug: langdb-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-analytics-api-openapi.yml
- filename: langdb-chat-api-openapi.yml
  format: yaml
  label: LangDB Chat API
  slug: langdb-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-chat-api-openapi.yml
- filename: langdb-embeddings-api-openapi.yml
  format: yaml
  label: LangDB Embeddings API
  slug: langdb-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-embeddings-api-openapi.yml
- filename: langdb-images-api-openapi.yml
  format: yaml
  label: LangDB Images API
  slug: langdb-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-images-api-openapi.yml
- filename: langdb-models-api-openapi.yml
  format: yaml
  label: LangDB Models API
  slug: langdb-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-models-api-openapi.yml
- filename: langdb-threads-api-openapi.yml
  format: yaml
  label: LangDB Threads API
  slug: langdb-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-threads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: LangDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LangDB
provider_slug: langdb
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'LangDB API key (project access token) sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/langdb-openapi.yml
  type: http
slug: langdb-authentication
source_filename: langdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langdb-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'LangDB API key (project access token) sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/langdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/authentication/langdb-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- AI Gateway
- Routing
- Governance
- MCP
---
