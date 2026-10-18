---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpnest-openapi-generated.yml
  format: yaml
  label: MCPNest API
  slug: mcpnest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpnest/refs/heads/main/openapi/_ae-authored/mcpnest-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mcpnest Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCPNest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MCPNest
provider_slug: mcpnest
scheme_count: 1
schemes:
- evidence: This MCP server allows users to interact with a PostgreSQL database through a secure GitHub OAuth authentication.
  name: GitHub OAuth
  type: oauth2
slug: mcpnest-authentication
source_filename: mcpnest-authentication.yml
source_heading: Authentication Profile
source_url: https://mcpnest.io/servers/remote-mcp-server-with-auth
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcpnest.io/servers/remote-mcp-server-with-auth\nsources:\n- https://mcpnest.io/servers/remote-mcp-server-with-auth\n- https://mcpnest.io/servers/mcp-chinese-getting-started-guide-1\nschemes:\n- type: oauth2\n  name: GitHub OAuth\n  evidence: This MCP server allows users to interact with a PostgreSQL database through a secure GitHub OAuth authentication.\ndocs: https://mcpnest.io/servers/remote-mcp-server-with-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpnest/refs/heads/main/authentication/mcpnest-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Cloud
- DevOps
- AI
---
