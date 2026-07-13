---
api_key_in: []
api_specs:
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Documents API
  slug: ragie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Retrievals API
  slug: ragie-retrievals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Connections API
  slug: ragie-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Entities and Extraction API
  slug: ragie-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Partitions API
  slug: ragie-partitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ragie Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ragie secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ragie
provider_slug: ragie-ai
scheme_count: 1
schemes:
- description: Ragie API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ragie-ai-openapi.yml
  type: http
slug: ragie-ai-authentication
source_filename: ragie-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ragie-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Ragie API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/ragie-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/authentication/ragie-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- RAG
- Retrieval
- Vector Search
- Document Ingestion
---
