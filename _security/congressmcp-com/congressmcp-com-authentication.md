---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CongressMCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: CongressMCP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CongressMCP
provider_slug: congressmcp-com
scheme_count: 2
schemes:
- applies_to: https://www.congressmcp.com/mcp
  flow: authorizationCode
  name: oauth2
  notes: Each authorization names the requested permissions (see scopes/congressmcp-com-scopes.yml). The docs say Devin's CLI "stores remote Streamable HTTP servers and supports OAuth/DCR", which points to dynamic client registration; the registration endpoint itself was not probed (probe-safety rules).
  pkce: true
  quote: OAuth 2.1 with PKCE is the preferred path. Access tokens are short-lived, refresh tokens rotate, and customers can revoke an entire connected app from their account.
  type: oauth2
- applies_to: https://www.congressmcp.com/mcp and /api/v1/workspaces/:wsId/research
  example_header: 'Authorization: Bearer <your-api-key>'
  header: Authorization
  name: apiKey
  notes: Keys are managed at /account; Indie and Pro plans state "One individual account with multiple API keys".
  quote: API keys remain available for clients that only support bearer headers.
  scheme: bearer
  type: http
slug: congressmcp-com-authentication
source_filename: congressmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://congressmcp.com/docs\ndocs: https://congressmcp.com/docs\nsummary: No OpenAPI is published; auth profile read from the docs. OAuth 2.1 with PKCE is the preferred path for the MCP endpoint, with revocable bearer API keys for clients that only support headers. The same API key or a web session authenticates the documented workspace research REST routes.\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  applies_to: https://www.congressmcp.com/mcp\n  quote: OAuth 2.1 with PKCE is the preferred path. Access tokens are short-lived, refresh tokens rotate, and customers can revoke an entire connected app from their account.\n  notes: Each authorization names the requested permissions (see scopes/congressmcp-com-scopes.yml). The docs say Devin's CLI \"stores remote Streamable HTTP servers and supports OAuth/DCR\", which points to dynamic client registration; the registration endpoint itself\
  \ was not probed (probe-safety rules).\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  applies_to: https://www.congressmcp.com/mcp and /api/v1/workspaces/:wsId/research\n  quote: API keys remain available for clients that only support bearer headers.\n  example_header: 'Authorization: Bearer <your-api-key>'\n  notes: Keys are managed at /account; Indie and Pro plans state \"One individual account with multiple API keys\".\n"
source_yaml_url: https://artifacts.apis.io/congressmcp-com/authentication/congressmcp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Legislation
- Government
- Congress
- State Legislatures
- Bill Tracking
- MCP
- Artificial Intelligence
- Policy Research
---
