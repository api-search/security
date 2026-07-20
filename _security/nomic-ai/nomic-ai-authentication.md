---
api_key_in: []
api_specs:
- filename: nomic-ai-openapi.yml
  format: yaml
  label: Nomic Atlas API
  slug: atlas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomic-ai/refs/heads/main/openapi/nomic-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nomic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nomic AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nomic AI
provider_slug: nomic-ai
scheme_count: 1
schemes:
- description: 'API key passed as a Bearer token in the Authorization header:

    `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nomic-ai-openapi.yml
  type: http
slug: nomic-ai-authentication
source_filename: nomic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nomic-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API key passed as a Bearer token in the Authorization header:\n    `Authorization: Bearer [example key]`.\n  sources:\n  - openapi/nomic-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomic-ai/refs/heads/main/authentication/nomic-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Embeddings
- Vector Database
- Data Exploration
- LLM
- Open Source
- RAG
- Atlas
---
