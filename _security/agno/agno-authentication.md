---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: AgentOS Agent API
  slug: agentos-api
  spec_type: OpenAPI
  url: https://docs.agno.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agno
provider_slug: agno
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/agno-agentos-api-openapi.yml
  type: http
slug: agno-authentication
source_filename: agno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agno-agentos-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/agno-agentos-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/authentication/agno-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Multi-Agent Systems
- Python Framework
- LLM
- Machine Learning
- Agentic AI
- Open Source
- Agent Runtime
---
