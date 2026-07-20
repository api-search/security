---
api_key_in:
- header
api_specs:
- filename: clawvisor-gateway-openapi.yml
  format: yaml
  label: Clawvisor Gateway API
  slug: clawvisor-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawvisor/refs/heads/main/openapi/clawvisor-gateway-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clawvisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clawvisor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clawvisor
provider_slug: clawvisor
scheme_count: 2
schemes:
- description: Agent token (or dashboard JWT for admin-gated endpoints), sent as Authorization Bearer header.
  name: agentToken
  scheme: bearer
  sources:
  - openapi/clawvisor-gateway-openapi.yml
  type: http
- description: Agent token for the skill catalog endpoint.
  in: header
  name: agentTokenHeader
  parameter: X-Clawvisor-Agent-Token
  sources:
  - openapi/clawvisor-gateway-openapi.yml
  type: apiKey
slug: clawvisor-authentication
source_filename: clawvisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/clawvisor-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: agentToken\n  type: http\n  scheme: bearer\n  description: Agent token (or dashboard JWT for admin-gated endpoints), sent as Authorization\n    Bearer header.\n  sources:\n  - openapi/clawvisor-gateway-openapi.yml\n- name: agentTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Clawvisor-Agent-Token\n  description: Agent token for the skill catalog endpoint.\n  sources:\n  - openapi/clawvisor-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawvisor/refs/heads/main/authentication/clawvisor-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Agents
- Authorization
- Security
- Identity
- Access Control
- MCP
- Credential Management
- Governance
- Developer Tools
---
