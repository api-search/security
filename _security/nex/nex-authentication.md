---
api_key_in:
- header
api_specs:
- filename: nex-openapi-original.json
  format: json
  label: Nex Developer API
  slug: nex-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nex
provider_slug: nex
scheme_count: 1
schemes:
- description: 'API key for authentication (format: "Bearer YOUR_API_KEY")'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/nex-openapi-original.json
  type: apiKey
slug: nex-authentication
source_filename: nex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nex-openapi-original.json\ndocs: https://docs.nex.ai/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  format: 'Authorization: Bearer sk-YOUR_API_KEY'\n  scopes_ref: scopes/nex-scopes.yml\n  note: >-\n    API keys are generated from the Nex web UI. Each key carries scopes that\n    gate operations (see scopes/nex-scopes.yml). End-user login to the Nex app\n    itself is brokered by WorkOS AuthKit, but the Developer API is API-key only.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key for authentication (format: \"Bearer YOUR_API_KEY\")'\n  sources:\n  - openapi/nex-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/authentication/nex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Agents
- Knowledge Graph
- Context
- Memory
- MCP
- Model Context Protocol
- Workflow Automation
- Integrations
- Developer API
---
