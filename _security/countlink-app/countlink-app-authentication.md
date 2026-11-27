---
anonymous_access: true
api_key_in: []
auth_types: []
description: CountLink's only programmatic surface, the MCP server at https://countlink.app/mcp, is documented as requiring no authentication and no account. The web app itself has no accounts ("No account, ever. There is nothing to sign up for and nothing to log into.").
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CountLink Authentication
name_suffix: Authentication
oauth_flows: []
overview: CountLink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CountLink
provider_slug: countlink-app
scheme_count: 1
schemes:
- applies_to: https://countlink.app/mcp
  evidence: '`https://countlink.app/mcp` is a Model Context Protocol server (JSON-RPC 2.0 over POST, no auth, no account).'
  type: none
slug: countlink-app-authentication
source_filename: countlink-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://countlink.app/llms.txt\ndocs: https://countlink.app/how-it-works\nname: CountLink authentication\ndescription: CountLink's only programmatic surface, the MCP server at https://countlink.app/mcp, is documented as requiring no authentication and no account. The web app itself has no accounts (\"No account, ever. There is nothing to sign up for and nothing to log into.\").\nschemes:\n- type: none\n  applies_to: https://countlink.app/mcp\n  evidence: '`https://countlink.app/mcp` is a Model Context Protocol server (JSON-RPC 2.0 over POST, no auth, no account).'\n"
source_yaml_url: https://artifacts.apis.io/countlink-app/authentication/countlink-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Countdown Timer
- Shared Timer
- Productivity
- Education
- Meetings
- MCP
- Web App
---
