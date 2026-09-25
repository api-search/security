---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avalix-ai-openapi.json
  format: json
  label: Autonoma Trust Gate API
  slug: autonoma-trust-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalix-ai/refs/heads/main/openapi/avalix-ai-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Avalix Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avalix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avalix
provider_slug: avalix-ai
scheme_count: 1
schemes:
- name: reportToken
  scheme: bearer
  sources:
  - openapi/avalix-ai-openapi.json
  type: http
slug: avalix-ai-authentication
source_filename: avalix-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/avalix-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: reportToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/avalix-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalix-ai/refs/heads/main/authentication/avalix-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- AI Trust
- Agent Security
- Data Validation
- AI Implementation
- Custom AI
- Agent-Native
---
