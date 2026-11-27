---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Command Mail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Command Mail declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Command Mail
provider_slug: commandmail-app
scheme_count: 3
schemes:
- applies_to: hosted MCP server https://commandmail.app/mcp
  description: Hosted MCP with OAuth. The browser authorization page lists each requested permission separately and the user can switch any off; mail:send starts switched off.
  name: oauth2
  type: oauth2
- applies_to: REST /api/...
  description: 'REST with a key carrying exactly the scopes you grant: GET https://commandmail.app/api/capabilities with Authorization: Bearer <key>. API keys are created and revoked in the API keys section of Settings; a key cannot manage other keys.'
  name: bearerApiKey
  scheme: bearer
  type: http
- applies_to: commandmail CLI and local MCP (commandmail mcp)
  description: The CLI authenticates with commandmail login; local MCP runs through the CLI using its login.
  name: cliLogin
  type: other
slug: commandmail-app-authentication
source_filename: commandmail-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commandmail.app/en/agents\ndocs: https://commandmail.app/en/docs/permissions-and-autonomy\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: hosted MCP server https://commandmail.app/mcp\n  description: Hosted MCP with OAuth. The browser authorization page lists each requested permission separately and the user can switch any off; mail:send starts switched off.\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  applies_to: REST /api/...\n  description: 'REST with a key carrying exactly the scopes you grant: GET https://commandmail.app/api/capabilities with Authorization: Bearer <key>. API keys are created and revoked in the API keys section of Settings; a key cannot manage other keys.'\n- name: cliLogin\n  type: other\n  applies_to: commandmail CLI and local MCP (commandmail mcp)\n  description: The CLI authenticates with commandmail login; local MCP runs through the CLI using its login.\nnotes:\n- Approving\
  \ drafts, deciding suggestions, changing autonomy, setting the daily send limit and managing API keys only work in a signed-in browser session; the server refuses these calls from a token.\n- Revocation: disconnecting an app under connected apps in Settings revokes every token that app holds.\n"
source_yaml_url: https://artifacts.apis.io/commandmail-app/authentication/commandmail-app-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Email
- AI Agents
- MCP
- Inbox
- Productivity
- Automation
---
