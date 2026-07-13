---
api_key_in: []
api_specs:
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Agents API
  slug: agno-agentos-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Teams API
  slug: agno-agentos-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Workflows API
  slug: agno-agentos-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Sessions API
  slug: agno-agentos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Memory API
  slug: agno-agentos-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Knowledge API
  slug: agno-agentos-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Evals API
  slug: agno-agentos-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agno Agi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agno
provider_slug: agno-agi
scheme_count: 1
schemes:
- description: HTTP Bearer token equal to OS_SECURITY_KEY. Required only when a Security Key is configured on the AgentOS instance; disabled otherwise.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agno-agi-openapi.yml
  type: http
slug: agno-agi-authentication
source_filename: agno-agi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agno-agi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: HTTP Bearer token equal to OS_SECURITY_KEY. Required only when a Security Key\n    is configured on the AgentOS instance; disabled otherwise.\n  sources:\n  - openapi/agno-agi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/authentication/agno-agi-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- Multi-Agent
- LLM
- Framework
- Open Source
- Runtime
---
