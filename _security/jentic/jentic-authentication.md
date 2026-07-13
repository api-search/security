---
api_key_in:
- header
api_specs:
- filename: jentic-openapi.yml
  format: yaml
  label: Jentic API
  slug: jentic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/openapi/jentic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jentic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jentic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jentic
provider_slug: jentic
scheme_count: 1
schemes:
- description: Agent-scoped API key obtained either by calling `/auth/register` or by clicking Generate API Key on an agent in the Jentic console at app.jentic.com. The key authorizes only the APIs and workflows in that agent's scope.
  in: header
  name: apiKeyAuth
  parameter: X-JENTIC-API-KEY
  sources:
  - openapi/jentic-openapi.yml
  type: apiKey
slug: jentic-authentication
source_filename: jentic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jentic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-JENTIC-API-KEY\n  description: Agent-scoped API key obtained either by calling `/auth/register` or by clicking\n    Generate API Key on an agent in the Jentic console at app.jentic.com. The key authorizes\n    only the APIs and workflows in that agent's scope.\n  sources:\n  - openapi/jentic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/authentication/jentic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agents
- Arazzo
- OpenAPI
- MCP
- Workflows
- Integrations
- Agent Runtime
- Standard Agent
- Just In Time Tooling
- Credential Vault
- Agent Governance
- Observability
- API AI Readiness
---
