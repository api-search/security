---
api_key_in:
- header
api_specs:
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Parse Task API
  slug: chunkr-parse-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Extract Task API
  slug: chunkr-extract-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Task Management API
  slug: chunkr-task-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Files API
  slug: chunkr-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Health and Extras API
  slug: chunkr-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chunkr Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chunkr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chunkr
provider_slug: chunkr-ai
scheme_count: 1
schemes:
- description: 'API key issued from the Chunkr dashboard, sent as the raw value of the Authorization header (e.g. "Authorization: lu_...").'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/chunkr-ai-openapi.yml
  type: apiKey
slug: chunkr-ai-authentication
source_filename: chunkr-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chunkr-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key issued from the Chunkr dashboard, sent as the raw value of the Authorization\n    header (e.g. \"Authorization: lu_...\").'\n  sources:\n  - openapi/chunkr-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/authentication/chunkr-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Parsing
- OCR
- Chunking
- RAG
- Document Intelligence
---
