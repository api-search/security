---
api_key_in:
- header
api_specs:
- filename: vellum-openapi.json
  format: json
  label: Vellum LLM Platform API
  slug: llm-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vellum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vellum AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vellum AI
provider_slug: vellum
scheme_count: 1
schemes:
- in: header
  name: default
  parameter: X-API-KEY
  sources:
  - openapi/vellum-openapi.json
  type: apiKey
slug: vellum-authentication
source_filename: vellum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vellum-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: default\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/vellum-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/authentication/vellum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- LLM Platform
- Prompt Engineering
- Workflows
- Evaluations
- LLM Ops
- RAG
- Observability
- Datasets
- Deployments
- Multi-Provider
- Agent Builder
- Self-Hosted
---
