---
api_key_in: []
api_specs:
- filename: inkeep-openapi.yml
  format: yaml
  label: Inkeep Chat Completions (RAG) API
  slug: inkeep-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inkeep/refs/heads/main/openapi/inkeep-openapi.yml
- filename: inkeep-openapi.yml
  format: yaml
  label: Inkeep Analytics API
  slug: inkeep-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inkeep/refs/heads/main/openapi/inkeep-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inkeep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inkeep secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inkeep
provider_slug: inkeep
scheme_count: 1
schemes:
- bearerFormat: Inkeep API key
  description: 'Bearer token using an API key created in the Inkeep dashboard under Projects > Assistants > Create assistant > API. Set the header `Authorization: Bearer <INKEEP_API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/inkeep-openapi.yml
  type: http
slug: inkeep-authentication
source_filename: inkeep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inkeep-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Inkeep API key\n  description: 'Bearer token using an API key created in the Inkeep dashboard under Projects\n    > Assistants > Create assistant > API. Set the header `Authorization: Bearer <INKEEP_API_KEY>`.'\n  sources:\n  - openapi/inkeep-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inkeep/refs/heads/main/authentication/inkeep-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Support
- RAG
- Agents
- Documentation
---
