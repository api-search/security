---
api_key_in:
- header
api_specs:
- filename: humanloop-openapi.yml
  format: yaml
  label: Humanloop LLM Platform API
  slug: llm-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanloop/refs/heads/main/openapi/humanloop-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Humanloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Humanloop secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Humanloop
provider_slug: humanloop
scheme_count: 2
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/humanloop-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/humanloop-openapi.yml
  type: apiKey
slug: humanloop-authentication
source_filename: humanloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/humanloop-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/humanloop-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/humanloop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanloop/refs/heads/main/authentication/humanloop-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- LLM Platform
- Prompt Management
- Evaluations
- LLM Ops
- Observability
- Datasets
- Prompts
- Tools
- Logs
- Multi-Provider
- Sunsetting
- Acquired
---
