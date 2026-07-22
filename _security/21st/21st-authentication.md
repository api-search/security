---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 21St Authentication
name_suffix: Authentication
oauth_flows: []
overview: 21st secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 21st
provider_slug: 21st
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter_name: x-api-key
  provisioning: https://21st.dev/magic/console
  type: apiKey
  used_by:
  - '@21st-dev/cli (--api-key flag)'
  - '@21st-dev/magic local MCP server (API_KEY_21ST)'
  - remote MCP server https://21st.dev/api/mcp (x-api-key header)
slug: 21st-authentication
source_filename: 21st-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://21st.dev/magic/console + https://github.com/21st-dev/magic-mcp + https://github.com/21st-dev/claude-code-plugin\nnote: >-\n  21st has no public REST OpenAPI; authentication is documented across the Magic console,\n  the Magic MCP server and the remote hosted MCP. A single API key minted in the console\n  authenticates the CLI, the local stdio MCP server and the remote HTTP MCP server. The\n  remote server transmits the key as the x-api-key request header; the local server and CLI\n  read it from the API_KEY_21ST environment variable / --api-key flag.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  header_name: x-api-key\n  env_var: API_KEY_21ST\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  provisioning: https://21st.dev/magic/console\n  used_by:\n  - \"@21st-dev/cli (--api-key flag)\"\n  - \"@21st-dev/magic local MCP server (API_KEY_21ST)\"\n  - remote\
  \ MCP server https://21st.dev/api/mcp (x-api-key header)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/21st/refs/heads/main/authentication/21st-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- UI Components
- React
- Model Context Protocol
- Developer Tools
- AI
- Agents
- Design Systems
- Frontend
- Component Registry
---
