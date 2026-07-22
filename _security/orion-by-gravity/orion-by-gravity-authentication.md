---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Orion By Gravity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orion by Gravity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orion by Gravity
provider_slug: orion-by-gravity
scheme_count: 1
schemes:
- description: The Orion remote MCP server authenticates via a browser-based OAuth login using the user's Orion credentials. Clients (Claude Code, Claude Desktop, Cursor, Windsurf) add the server URL and complete an interactive authentication flow — no static API key or manual token is issued to the client.
  flow: browser-based authorization
  name: MCP OAuth (browser login)
  server: https://g.runorion.com/mcp
  sources:
  - https://docs.runorion.com/mcp/setup.md
  transport: http
  type: oauth2
slug: orion-by-gravity-authentication
source_filename: orion-by-gravity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.runorion.com/mcp/setup.md\ndocs: https://docs.runorion.com/mcp/setup.md\nsummary:\n  types: [oauth2]\n  flows: [browser-login]\n  surface: mcp\nschemes:\n- name: MCP OAuth (browser login)\n  type: oauth2\n  flow: browser-based authorization\n  transport: http\n  server: https://g.runorion.com/mcp\n  description: >-\n    The Orion remote MCP server authenticates via a browser-based OAuth login using the user's Orion\n    credentials. Clients (Claude Code, Claude Desktop, Cursor, Windsurf) add the server URL and complete\n    an interactive authentication flow — no static API key or manual token is issued to the client.\n  sources: [https://docs.runorion.com/mcp/setup.md]\nnotes: >-\n  Orion is a commercial SaaS product with no documented public REST/OpenAPI surface; its programmatic\n  access is the MCP server, which brokers authentication through the interactive OAuth login above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion-by-gravity/refs/heads/main/authentication/orion-by-gravity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Analytics
- Business Intelligence
- Artificial Intelligence
- Data
- MCP
- Data Warehouse
- SaaS
---
