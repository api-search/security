---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Clino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clino declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clino
provider_slug: clino-ch
scheme_count: 1
schemes:
- applies_to: https://clino.ch/mcp
  description: 'The MCP server is public and unauthenticated: "Any MCP client connects without a key, CORS is open, every answer has a JSON schema." The repo README tells ChatGPT users to create the connector with "no authentication".'
  evidence:
  - https://clino.ch/en/mcp
  - https://github.com/salvador-creator/clino-mcp
  id: none
  type: none
slug: clino-ch-authentication
source_filename: clino-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clino.ch/en/mcp\ndocs: https://clino.ch/en/mcp\nschemes:\n- id: none\n  type: none\n  applies_to: https://clino.ch/mcp\n  description: 'The MCP server is public and unauthenticated: \"Any MCP client connects without a key, CORS is open, every answer has a JSON schema.\" The repo README tells ChatGPT users to create the connector with \"no authentication\".'\n  evidence:\n  - https://clino.ch/en/mcp\n  - https://github.com/salvador-creator/clino-mcp\nnote: The paid Clino web app uses an account login (https://clino.ch/de/login); it has no documented public API, so no scheme is recorded for it.\n"
source_yaml_url: https://artifacts.apis.io/clino-ch/authentication/clino-ch-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payroll
- Household Employment
- Domestic Workers
- Social Security
- Switzerland
- Human Resources
- MCP
---
