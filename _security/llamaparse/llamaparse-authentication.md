---
api_key_in: []
api_specs:
- filename: llamaparse-llamacloud-openapi.yml
  format: yaml
  label: LlamaParse Parse API
  slug: llamaparse-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaparse/refs/heads/main/openapi/llamaparse-llamacloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Llamaparse Authentication
name_suffix: Authentication
oauth_flows: []
overview: LlamaParse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LlamaParse
provider_slug: llamaparse
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/llamaparse-llamacloud-openapi.yml
  type: http
slug: llamaparse-authentication
source_filename: llamaparse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/llamaparse-llamacloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/llamaparse-llamacloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llamaparse/refs/heads/main/authentication/llamaparse-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Parsing
- OCR
- PDF
- LLM
- RAG
- AI
- Document Intelligence
- Structured Data Extraction
---
