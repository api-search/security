---
api_key_in: []
api_specs:
- filename: flowise-openapi.yml
  format: yaml
  label: Flowise API
  slug: flowise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flowise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flowise
provider_slug: flowise
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flowise-openapi.yml
  type: http
slug: flowise-authentication
source_filename: flowise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flowise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/flowise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/authentication/flowise-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Agent Workflows
- Artificial Intelligence
- Large Language Models
- Low Code
- Visual Builder
- LangChain
- RAG
- Retrieval Augmented Generation
- Chatbots
- Open Source
- Node.js
- TypeScript
---
