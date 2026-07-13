---
api_key_in:
- header
api_specs:
- filename: unstructured-platform-api-openapi.yml
  format: yaml
  label: Unstructured Platform API
  slug: unstructured-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-platform-api-openapi.yml
- filename: unstructured-partition-endpoint-openapi.yml
  format: yaml
  label: Unstructured Partition Endpoint
  slug: unstructured-partition-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-partition-endpoint-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unstructured Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unstructured secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unstructured
provider_slug: unstructured
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: unstructured-api-key
  sources:
  - openapi/unstructured-partition-endpoint-openapi.yml
  type: apiKey
slug: unstructured-authentication
source_filename: unstructured-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unstructured-partition-endpoint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: unstructured-api-key\n  sources:\n  - openapi/unstructured-partition-endpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/authentication/unstructured-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- document-processing
- ETL
- RAG
- LLM
- PDF
- OCR
- data-ingestion
- chunking
- embeddings
- AI
---
