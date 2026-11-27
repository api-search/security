---
anonymous_access: false
api_key_in: []
api_specs:
- filename: callsyncapp-com-openapi-generated.yml
  format: yaml
  label: CallSync API
  slug: callsyncapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callsyncapp-com/openapi/_ae-authored/callsyncapp-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CallSync Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallSync declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CallSync
provider_slug: callsyncapp-com
scheme_count: 2
schemes:
- applies_to: REST API https://mcp.callsyncapp.com/api/v1
  description: 'Workspace API key created in the dashboard under API & Apps and sent as "Authorization: Bearer" header.'
  evidence: 'Copy the key. Store it in your server’s environment as CALLSYNC_API_KEY. Send it in the Authorization: Bearer header.'
  key_management:
    rotation: Regenerating it invalidates the current key; update every integration that uses it.
    storage: Keep the key outside browser code, mobile bundles and public repositories.
  name: bearerApiKey
  scheme: bearer
  type: http
- applies_to: Remote MCP server https://mcp.callsyncapp.com/connect
  description: MCP clients sign in with OAuth; the docs describe automatic client registration ("Register automatically" under OAuth client in Claude).
  evidence: Use the sign-in/OAuth flow offered by CallSync.
  name: mcpOAuth
  scopes_documented: false
  source: https://help.callsyncapp.com/connect-ai-agent/
  type: oauth2
slug: callsyncapp-com-authentication
source_filename: callsyncapp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://help.callsyncapp.com/api-guide/\ndocs: https://help.callsyncapp.com/api-guide/\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  applies_to: REST API https://mcp.callsyncapp.com/api/v1\n  description: 'Workspace API key created in the dashboard under API & Apps and sent as \"Authorization: Bearer\" header.'\n  evidence: \"Copy the key. Store it in your server’s environment as CALLSYNC_API_KEY. Send it in the Authorization: Bearer header.\"\n  key_management:\n    rotation: \"Regenerating it invalidates the current key; update every integration that uses it.\"\n    storage: Keep the key outside browser code, mobile bundles and public repositories.\n- name: mcpOAuth\n  type: oauth2\n  applies_to: Remote MCP server https://mcp.callsyncapp.com/connect\n  description: MCP clients sign in with OAuth; the docs describe automatic client registration (\"Register automatically\" under OAuth client in Claude).\n\
  \  source: https://help.callsyncapp.com/connect-ai-agent/\n  evidence: \"Use the sign-in/OAuth flow offered by CallSync.\"\n  scopes_documented: false\nnote: No OAuth scope list is published; authorized apps are managed in CallSync → API & Apps.\n"
source_yaml_url: https://artifacts.apis.io/callsyncapp-com/authentication/callsyncapp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Call Tracking
- Call Recording
- Android
- Sales CRM
- Webhook
- MCP
- AI Agents
---
