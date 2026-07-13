---
api_key_in: []
api_specs:
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Indexes and Collections
  slug: indexes-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Search
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Answer Sessions (RAG)
  slug: answer-sessions-rag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orama secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orama
provider_slug: orama
scheme_count: 1
schemes:
- description: 'Private (write) API key sent as `Authorization: Bearer {key}` for management and ingestion endpoints on api.askorama.ai. Search and answer endpoints instead use a public (read) API key supplied via the `api-key` query parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/orama-openapi.yml
  type: http
slug: orama-authentication
source_filename: orama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orama-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Private (write) API key sent as `Authorization: Bearer {key}` for management\n    and ingestion endpoints on api.askorama.ai. Search and answer endpoints instead use a public\n    (read) API key supplied via the `api-key` query parameter.'\n  sources:\n  - openapi/orama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/authentication/orama-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Vector Search
- RAG
- Open Source
- Search as a Service
---
