---
api_key_in: []
api_specs:
- filename: glama-openapi.yml
  format: yaml
  label: Glama MCP Marketplace & Gateway
  slug: mcp-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glama AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glama AI
provider_slug: glama
scheme_count: 1
schemes:
- bearerFormat: Glama API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/glama-openapi.yml
  type: http
slug: glama-authentication
source_filename: glama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glama-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Glama API Key\n  sources:\n  - openapi/glama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/authentication/glama-authentication.yml
summary_line: http · 1 scheme
tags:
- MCP
- Model Context Protocol
- MCP Marketplace
- MCP Gateway
- MCP Hosting
- MCP Inspector
- AI Gateway
- LLM Gateway
- Connectors
- OAuth
- Observability
- Multi-Provider
---
