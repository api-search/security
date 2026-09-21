---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: decision-anchor-com-openapi.yml
  format: yaml
  label: Decision Anchor API
  slug: decision-anchor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decision-anchor-com/refs/heads/main/openapi/decision-anchor-com-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Decision Anchor Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Decision Anchor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Decision Anchor
provider_slug: decision-anchor-com
scheme_count: 2
schemes:
- description: Agent auth_token issued at registration (POST /v1/agent/register). Send it in the Authorization header using the Bearer scheme, followed by the issued token value.
  name: AgentToken
  scheme: bearer
  sources:
  - openapi/decision-anchor-com-openapi.yml
  type: http
- description: Session cookie issued after DAP login
  in: cookie
  name: DAPSession
  parameter: connect.sid
  sources:
  - openapi/decision-anchor-com-openapi.yml
  type: apiKey
slug: decision-anchor-com-authentication
source_filename: decision-anchor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/decision-anchor-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: AgentToken\n  type: http\n  scheme: bearer\n  description: Agent auth_token issued at registration (POST /v1/agent/register). Send it in\n    the Authorization header using the Bearer scheme, followed by the issued token value.\n  sources:\n  - openapi/decision-anchor-com-openapi.yml\n- name: DAPSession\n  type: apiKey\n  in: cookie\n  parameter: connect.sid\n  description: Session cookie issued after DAP login\n  sources:\n  - openapi/decision-anchor-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decision-anchor-com/refs/heads/main/authentication/decision-anchor-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Agents
- Agent Accountability
- Decision Records
- Audit Trail
- A2A
- MCP
- x402
- Agentic Commerce
- Multi-Agent Systems
- agent-native
- South Korea
---
