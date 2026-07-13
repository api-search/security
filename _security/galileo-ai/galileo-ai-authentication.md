---
api_key_in:
- header
api_specs:
- filename: galileo-ai-openapi.yml
  format: yaml
  label: Galileo Public API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Galileo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Galileo secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Galileo
provider_slug: galileo-ai
scheme_count: 3
schemes:
- in: header
  name: apiKeyHeader
  parameter: Galileo-API-Key
  sources:
  - openapi/galileo-ai-openapi.yml
  type: apiKey
- description: OAuth 2.0 password bearer (JWT) issued by /v2/token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/galileo-ai-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/galileo-ai-openapi.yml
  type: http
slug: galileo-ai-authentication
source_filename: galileo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/galileo-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Galileo-API-Key\n  sources:\n  - openapi/galileo-ai-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 password bearer (JWT) issued by /v2/token\n  sources:\n  - openapi/galileo-ai-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/galileo-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/authentication/galileo-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI Evaluation
- AI Observability
- GenAI
- Guardrails
- Agentic AI
- LLM
- Tracing
- Experiments
- Prompts
- Datasets
---
