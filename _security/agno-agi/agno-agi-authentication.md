---
api_key_in: []
api_specs:
- filename: agno-agi-agents-api-openapi.yml
  format: yaml
  label: Agno Agents API
  slug: agno-agi-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-agents-api-openapi.yml
- filename: agno-agi-evals-api-openapi.yml
  format: yaml
  label: Agno Evals API
  slug: agno-agi-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-evals-api-openapi.yml
- filename: agno-agi-knowledge-api-openapi.yml
  format: yaml
  label: Agno Knowledge API
  slug: agno-agi-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-knowledge-api-openapi.yml
- filename: agno-agi-memory-api-openapi.yml
  format: yaml
  label: Agno Memory API
  slug: agno-agi-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-memory-api-openapi.yml
- filename: agno-agi-sessions-api-openapi.yml
  format: yaml
  label: Agno Sessions API
  slug: agno-agi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-sessions-api-openapi.yml
- filename: agno-agi-teams-api-openapi.yml
  format: yaml
  label: Agno Teams API
  slug: agno-agi-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-teams-api-openapi.yml
- filename: agno-agi-workflows-api-openapi.yml
  format: yaml
  label: Agno Workflows API
  slug: agno-agi-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-workflows-api-openapi.yml
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
- Artificial Intelligence
- Agents
- Multi-Agent
- LLM
- Framework
- Open-Source
- Runtime
---
