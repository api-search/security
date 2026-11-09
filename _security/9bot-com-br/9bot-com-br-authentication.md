---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 9bot-com-br-discovery-api-openapi.yml
  format: yaml
  label: 9bot Discovery API
  slug: 9bot-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-discovery-api-openapi.yml
- filename: 9bot-com-br-health-api-openapi.yml
  format: yaml
  label: 9bot Health API
  slug: 9bot-com-br-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-health-api-openapi.yml
- filename: 9bot-com-br-mcp-api-openapi.yml
  format: yaml
  label: 9bot MCP API
  slug: 9bot-com-br-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 9Bot Com Br Authentication
name_suffix: Authentication
oauth_flows: []
overview: 9bot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 9bot
provider_slug: 9bot-com-br
scheme_count: 1
schemes:
- description: OAuth 2.1 Authorization Code flow with PKCE for agents.
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.9bot.com.br/oauth/authorize
      refreshUrl: https://mcp.9bot.com.br/oauth/revoke
      scopes: {}
      tokenUrl: https://mcp.9bot.com.br/oauth/token
  type: oauth2
slug: 9bot-com-br-authentication
source_filename: 9bot-com-br-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://9bot.com.br/auth.md\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 Authorization Code flow with PKCE for agents.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.9bot.com.br/oauth/authorize\n        tokenUrl: https://mcp.9bot.com.br/oauth/token\n        refreshUrl: https://mcp.9bot.com.br/oauth/revoke\n        scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/9bot-com-br/authentication/9bot-com-br-authentication.yml
summary_line: 1 scheme
tags:
- WhatsApp
- Automation
- Bot
- Messaging
- Integration
---
