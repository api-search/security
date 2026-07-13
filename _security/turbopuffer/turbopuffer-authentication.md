---
api_key_in: []
api_specs:
- filename: turbopuffer-openapi.yml
  format: yaml
  label: turbopuffer REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbopuffer/main/openapi/turbopuffer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turbopuffer Authentication
name_suffix: Authentication
oauth_flows: []
overview: turbopuffer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: turbopuffer
provider_slug: turbopuffer
scheme_count: 1
schemes:
- bearerFormat: API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/turbopuffer-openapi.yml
  type: http
slug: turbopuffer-authentication
source_filename: turbopuffer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turbopuffer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/turbopuffer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbopuffer/refs/heads/main/authentication/turbopuffer-authentication.yml
summary_line: http · 1 scheme
tags:
- Vector Search
- Full-Text Search
- Hybrid Search
- BM25
- Serverless
- Object Storage
- RAG
- Semantic Search
- AI Infrastructure
- Embeddings
---
