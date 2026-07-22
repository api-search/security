---
api_key_in: []
auth_types: []
description: How programmatic clients authenticate to Macro. Macro's public programmatic surface is its hosted MCP server; clients authenticate with OAuth via a browser sign-in when the MCP client first connects. There is no documented public REST API key scheme.
kind: authentication
layout: security
method: searched
name: Macro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Macro
provider_slug: macro
scheme_count: 1
schemes:
- applies_to: https://mcp-server.macro.com/mcp
  description: Authentication happens through Macro's OAuth flow when the MCP client connects. The user logs in via the browser during the initial connection. MCP access is available on all plans including free.
  flow: authorization_code
  id: mcp_oauth
  interaction: browser
  type: oauth2
slug: macro-authentication
source_filename: macro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.macro.com/AI/mcp/overview.md\nname: Macro Authentication\ntype: Authentication\ndescription: >-\n  How programmatic clients authenticate to Macro. Macro's public programmatic surface\n  is its hosted MCP server; clients authenticate with OAuth via a browser sign-in when\n  the MCP client first connects. There is no documented public REST API key scheme.\ndocs: https://docs.macro.com/AI/mcp/overview.md\nschemes:\n- id: mcp_oauth\n  type: oauth2\n  flow: authorization_code\n  interaction: browser\n  applies_to: https://mcp-server.macro.com/mcp\n  description: >-\n    Authentication happens through Macro's OAuth flow when the MCP client connects.\n    The user logs in via the browser during the initial connection. MCP access is\n    available on all plans including free.\nconnected_accounts:\n- provider: Gmail\n  purpose: Email sync (keyboard-driven email with Gmail sync)\n  docs: https://docs.macro.com/product/email.md\n\
  - provider: GitHub\n  purpose: Link pull requests to tasks; third-party OAuth approval required\n  docs: https://docs.macro.com/integrations/github.md\nnotes: >-\n  Macro is an end-user workspace application (desktop/iOS/web) rather than a developer\n  API platform; the primary agent-facing authenticated entry point is the MCP server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macro/refs/heads/main/authentication/macro-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Productivity
- Email
- Collaboration
- Workspace
- CRM
- Tasks
- AI Agents
- MCP
- Open Source
---
