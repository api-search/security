---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Courts.tennis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Courts.tennis declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Courts.tennis
provider_slug: courts-tennis
scheme_count: 1
schemes:
- applies_to:
  - https://www.courts.tennis/mcp
  description: The MCP endpoint takes no credentials. llms.txt states "Endpoint https://www.courts.tennis/mcp (Streamable HTTP, no authentication, read-only)" and the server card at https://www.courts.tennis/.well-known/mcp.json declares "authentication" {"type" "none"}.
  name: none
  type: none
slug: courts-tennis-authentication
source_filename: courts-tennis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.courts.tennis/llms.txt\ndocs: https://www.courts.tennis/llms.txt\nschemes:\n- type: none\n  name: none\n  description: The MCP endpoint takes no credentials. llms.txt states \"Endpoint https://www.courts.tennis/mcp (Streamable HTTP, no authentication, read-only)\" and the server card at https://www.courts.tennis/.well-known/mcp.json declares \"authentication\" {\"type\" \"none\"}.\n  applies_to:\n  - https://www.courts.tennis/mcp\nevidence:\n- url: https://www.courts.tennis/llms.txt\n  status: 200\n- url: https://www.courts.tennis/.well-known/mcp.json\n  status: 200\nnote: No OAuth, API keys or accounts exist. The terms page states \"Reading it needs no account, and there is nothing to buy.\"\n"
source_yaml_url: https://artifacts.apis.io/courts-tennis/authentication/courts-tennis-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Tennis
- Sports
- Sports Facilities
- Directories
- Open Data
- MCP
- Travel
---
