---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Solarscope Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: solarscope-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: solarscope-io
provider_slug: solarscope-io
scheme_count: 2
schemes:
- description: OAuth 2.1 dynamic client registration for MCP server
  flow: authorizationCode
  tokenUrl: https://solarscope.io/oauth/token
  type: oauth2
- description: Bearer <API key> for REST API
  in: header
  name: Authorization
  type: apiKey
slug: solarscope-io-authentication
source_filename: solarscope-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://solarscope.io/ai-agents\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    description: \"OAuth 2.1 dynamic client registration for MCP server\"\n    tokenUrl: \"https://solarscope.io/oauth/token\" # not explicitly given, placeholder? need actual? Not in page. We'll note not provided.\n  - type: apiKey\n    in: header\n    name: Authorization\n    description: \"Bearer <API key> for REST API\"\n"
source_yaml_url: https://artifacts.apis.io/solarscope-io/authentication/solarscope-io-authentication.yml
summary_line: 2 schemes
tags:
- Solar
- AI
- Renewable-Energy
- Site-Screening
- Mapping
---
