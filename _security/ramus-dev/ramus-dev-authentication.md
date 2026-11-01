---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ramus Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: ramus-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ramus-dev
provider_slug: ramus-dev
scheme_count: 2
schemes:
- description: API key set in environment variable RAMUS_API_KEY for CLI and agents.
  in: header
  name: RAMUS_API_KEY
  type: apiKey
- description: MCP OAuth flow for agents and integrations.
  flows:
    authorizationCode:
      authorizationUrl: https://ramus.dev/login
      scopes: {}
      tokenUrl: https://ramus.dev/api/mcp/oauth/token
  type: oauth2
slug: ramus-dev-authentication
source_filename: ramus-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://ramus.dev/docs/agents\nschemes:\n  - type: apiKey\n    name: RAMUS_API_KEY\n    in: header\n    description: API key set in environment variable RAMUS_API_KEY for CLI and agents.\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://ramus.dev/login\n        tokenUrl: https://ramus.dev/api/mcp/oauth/token\n        scopes: {}\n    description: MCP OAuth flow for agents and integrations.\n"
source_yaml_url: https://artifacts.apis.io/ramus-dev/authentication/ramus-dev-authentication.yml
summary_line: 2 schemes
tags:
- Android
- Emulator
- Cloud
- DeveloperTools
- API
---
