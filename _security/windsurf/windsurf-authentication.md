---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Windsurf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windsurf secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Windsurf
provider_slug: windsurf
scheme_count: 1
schemes:
- description: Service key authentication for Windsurf enterprise deployments
  in: header
  name: serviceKey
  parameter: Authorization
  sources:
  - openapi/windsurf-openapi.yml
  type: apiKey
slug: windsurf-authentication
source_filename: windsurf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windsurf-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: serviceKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Service key authentication for Windsurf enterprise deployments\n  sources:\n  - openapi/windsurf-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windsurf/refs/heads/main/authentication/windsurf-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Developer Tools
- Code Editor
- Agent
- Cascade
- IDE
- MCP
---
