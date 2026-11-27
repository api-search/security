---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Coco Pier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coco Pier declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coco Pier
provider_slug: coco-pier-com
scheme_count: 1
schemes:
- applies_to:
  - https://fx.coco-pier.com/mcp
  - GET /api/v1/summary
  description: The hosted remote MCP server and REST endpoint require no credentials.
  name: anonymous
  quote: FXContext is a hosted remote MCP server at https://fx.coco-pier.com/mcp . No account, sign-in, or API key is needed.
  type: none
slug: coco-pier-com-authentication
source_filename: coco-pier-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coco-pier.com/docs/\ndocs: https://coco-pier.com/docs/#connect\nschemes:\n- type: none\n  name: anonymous\n  description: The hosted remote MCP server and REST endpoint require no credentials.\n  quote: 'FXContext is a hosted remote MCP server at https://fx.coco-pier.com/mcp . No account, sign-in, or API key is needed.'\n  applies_to:\n  - https://fx.coco-pier.com/mcp\n  - GET /api/v1/summary\nnote: 'The docs also state for MCP clients \"Authentication: none\", and that the frontend \"does not create accounts, issue API keys\". No OAuth, so no scopes artifact.'\n"
source_yaml_url: https://artifacts.apis.io/coco-pier-com/authentication/coco-pier-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Foreign Exchange
- Macroeconomics
- Financial Data
- Central Banks
- Economic Calendar
- MCP
- AI Agents
---
