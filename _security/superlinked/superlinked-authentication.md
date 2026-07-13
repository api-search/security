---
api_key_in:
- header
api_specs:
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Ingestion API
  slug: superlinked-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Query API
  slug: superlinked-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Data Loader API
  slug: superlinked-data-loader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Superlinked Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superlinked secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Superlinked
provider_slug: superlinked
scheme_count: 2
schemes:
- description: Optional API key header. The open-source Superlinked Server ships without built-in auth; deployments commonly place an API key or bearer token check in front of it (gateway or custom middleware). Configure to match your deployment.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/superlinked-openapi.yml
  type: apiKey
- description: Optional bearer token, when the deployment fronts the server with token auth.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/superlinked-openapi.yml
  type: http
slug: superlinked-authentication
source_filename: superlinked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/superlinked-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Optional API key header. The open-source Superlinked Server ships without built-in\n    auth; deployments commonly place an API key or bearer token check in front of it (gateway\n    or custom middleware). Configure to match your deployment.\n  sources:\n  - openapi/superlinked-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional bearer token, when the deployment fronts the server with token auth.\n  sources:\n  - openapi/superlinked-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/authentication/superlinked-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Vectors
- Embeddings
- Vector Search
- Retrieval
- Recommendations
- RAG
---
