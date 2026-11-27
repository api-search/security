---
anonymous_access: true
api_key_in: []
api_specs:
- filename: taasky-ai-openapi-generated.yml
  format: yaml
  label: Taasky API
  slug: taasky-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taasky-ai/openapi/_ae-authored/taasky-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Taasky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taasky declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Taasky
provider_slug: taasky-ai
scheme_count: 2
schemes:
- description: No credentials required for keyless access using room tokens.
  type: none
- description: OAuth2 flow for account access via https://mcp.taasky.ai/mcp/account.
  flows:
    authorizationCode:
      authorizationUrl: <to be discovered>
      scopes: {}
      tokenUrl: <to be discovered>
  type: oauth2
slug: taasky-ai-authentication
source_filename: taasky-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: searched\nsource: https://docs.taasky.ai/reference/authentication.md\nschemes:\n  - type: none\n    description: No credentials required for keyless access using room tokens.\n  - type: oauth2\n    description: OAuth2 flow for account access via https://mcp.taasky.ai/mcp/account.\n    flows:\n      authorizationCode:\n        authorizationUrl: <to be discovered>\n        tokenUrl: <to be discovered>\n        scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/taasky-ai/authentication/taasky-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- MCP
- Automation
- Negotiation
---
