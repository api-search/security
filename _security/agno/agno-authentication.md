---
api_key_in: []
api_specs:
- filename: agno-a2a-api-openapi.yml
  format: yaml
  label: Agno A2A API
  slug: agno-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-a2a-api-openapi.yml
- filename: agno-agents-api-openapi.yml
  format: yaml
  label: Agno Agents API
  slug: agno-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-agents-api-openapi.yml
- filename: agno-agui-api-openapi.yml
  format: yaml
  label: Agno AGUI API
  slug: agno-agui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-agui-api-openapi.yml
- filename: agno-approvals-api-openapi.yml
  format: yaml
  label: Agno Approvals API
  slug: agno-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-approvals-api-openapi.yml
- filename: agno-components-api-openapi.yml
  format: yaml
  label: Agno Components API
  slug: agno-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-components-api-openapi.yml
- filename: agno-core-api-openapi.yml
  format: yaml
  label: Agno Core API
  slug: agno-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-core-api-openapi.yml
- filename: agno-database-api-openapi.yml
  format: yaml
  label: Agno Database API
  slug: agno-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-database-api-openapi.yml
- filename: agno-evals-api-openapi.yml
  format: yaml
  label: Agno Evals API
  slug: agno-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-evals-api-openapi.yml
- filename: agno-health-api-openapi.yml
  format: yaml
  label: Agno Health API
  slug: agno-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-health-api-openapi.yml
- filename: agno-home-api-openapi.yml
  format: yaml
  label: Agno Home API
  slug: agno-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-home-api-openapi.yml
- filename: agno-knowledge-api-openapi.yml
  format: yaml
  label: Agno Knowledge API
  slug: agno-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-knowledge-api-openapi.yml
- filename: agno-memory-api-openapi.yml
  format: yaml
  label: Agno Memory API
  slug: agno-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-memory-api-openapi.yml
- filename: agno-metrics-api-openapi.yml
  format: yaml
  label: Agno Metrics API
  slug: agno-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-metrics-api-openapi.yml
- filename: agno-registry-api-openapi.yml
  format: yaml
  label: Agno Registry API
  slug: agno-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-registry-api-openapi.yml
- filename: agno-schedules-api-openapi.yml
  format: yaml
  label: Agno Schedules API
  slug: agno-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-schedules-api-openapi.yml
- filename: agno-sessions-api-openapi.yml
  format: yaml
  label: Agno Sessions API
  slug: agno-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-sessions-api-openapi.yml
- filename: agno-slack-api-openapi.yml
  format: yaml
  label: Agno Slack API
  slug: agno-slack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-slack-api-openapi.yml
- filename: agno-teams-api-openapi.yml
  format: yaml
  label: Agno Teams API
  slug: agno-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-teams-api-openapi.yml
- filename: agno-traces-api-openapi.yml
  format: yaml
  label: Agno Traces API
  slug: agno-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-traces-api-openapi.yml
- filename: agno-whatsapp-api-openapi.yml
  format: yaml
  label: Agno Whatsapp API
  slug: agno-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-whatsapp-api-openapi.yml
- filename: agno-workflows-api-openapi.yml
  format: yaml
  label: Agno Workflows API
  slug: agno-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno/refs/heads/main/openapi/agno-workflows-api-openapi.yml
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
- Machine-Learning
- Agentic AI
- Open-Source
- Agent Runtime
---
