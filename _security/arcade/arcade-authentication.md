---
api_key_in:
- header
api_specs:
- filename: arcade-engine-openapi.yml
  format: yaml
  label: Arcade Engine API
  slug: arcade-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade/refs/heads/main/openapi/arcade-engine-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arcade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcade
provider_slug: arcade
scheme_count: 1
schemes:
- description: 'Enter your API key or API token in the format: Bearer <token>'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/arcade-engine-openapi.yml
  type: apiKey
slug: arcade-authentication
source_filename: arcade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcade-engine-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Enter your API key or API token in the format: Bearer <token>'\n  sources:\n  - openapi/arcade-engine-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcade/refs/heads/main/authentication/arcade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agents
- MCP
- AI Agents
- Authorization
- OAuth
- Tool Calling
- Agent Infrastructure
- LLM
- Integrations
---
