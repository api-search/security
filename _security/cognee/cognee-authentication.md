---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Cognee REST API
  slug: cognee-rest-api
  spec_type: OpenAPI
  url: https://api.cognee.ai/docs
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cognee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognee secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cognee
provider_slug: cognee
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token authentication for self-hosted instances
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cognee-rest-api-openapi.yml
  type: http
- description: API key authentication for Cognee Cloud deployments
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/cognee-rest-api-openapi.yml
  type: apiKey
slug: cognee-authentication
source_filename: cognee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognee-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication for self-hosted instances\n  sources:\n  - openapi/cognee-rest-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key authentication for Cognee Cloud deployments\n  sources:\n  - openapi/cognee-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognee/refs/heads/main/authentication/cognee-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Memory
- Knowledge Graph
- RAG
- Agents
- Graph Database
- Vector Search
- LLM
- Open Source
---
