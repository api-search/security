---
api_key_in: []
auth_types: []
description: Bearer API keys in the Authorization header, plus a separate MCP-Token header for the MCP surface.
kind: authentication
layout: security
method: searched
name: Amuncore Authentication
name_suffix: Authentication
oauth_flows: []
overview: AmunCore declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AmunCore
provider_slug: amuncore
scheme_count: 2
schemes:
- example: 'Authorization: Bearer ak_live_…'
  header: Authorization
  id: bearer
  note: Shown on the homepage live-request demo.
  scheme: bearer
  type: http
- id: mcp-token
  in: header
  name: MCP-Token
  note: Required by the MCP endpoint; confirmed by its 401 error message.
  type: apiKey
slug: amuncore-authentication
source_filename: amuncore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-03'\nmethod: searched\nstatus: published\nsource: https://amuncore.com\ndescription: Bearer API keys in the Authorization header, plus a separate MCP-Token\n  header for the MCP surface.\nverified: '2026-08-03'\nschemes:\n- id: bearer\n  type: http\n  scheme: bearer\n  header: Authorization\n  example: 'Authorization: Bearer ak_live_…'\n  note: Shown on the homepage live-request demo.\n- id: mcp-token\n  type: apiKey\n  in: header\n  name: MCP-Token\n  note: Required by the MCP endpoint; confirmed by its 401 error message.\nsignup:\n  url: https://amuncore.com\n  free_plan: true\n  note: '\"Create free account\" / \"Free plan forever\" per the homepage.'\nevidence:\n- url: https://amuncore.com\n  status: 200\n- url: https://amuncore.com/mcp\n  status: 401\n  method: POST\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/authentication/amuncore-authentication.yml
summary_line: 2 schemes
tags:
- Database
- API Management
- Backend
- No Code
- SQL
- PostgreSQL
- MySQL
- Oracle
- MCP
- Agents
- Data
---
