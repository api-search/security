---
api_key_in: []
api_specs:
- filename: klavis-openapi.yml
  format: yaml
  label: Klavis MCP Platform API
  slug: mcp-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klavis/refs/heads/main/openapi/klavis-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Klavis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klavis AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klavis AI
provider_slug: klavis
scheme_count: 1
schemes:
- description: Klavis account API key passed via the Authorization Bearer header
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/klavis-openapi.yml
  type: http
slug: klavis-authentication
source_filename: klavis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klavis-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Klavis account API key passed via the Authorization Bearer header\n  sources:\n  - openapi/klavis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klavis/refs/heads/main/authentication/klavis-authentication.yml
summary_line: http · 1 scheme
tags:
- MCP
- Model Context Protocol
- MCP Servers
- MCP Hosting
- Connectors
- OAuth
- Sandboxes
- Agent Training
- Reinforcement Learning
- White Label
- Open Source
- Strata
---
