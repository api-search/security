---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentdocs-eu-openapi-generated.yml
  format: yaml
  label: agentdocs-eu API
  slug: agentdocs-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdocs-eu/openapi/_ae-authored/agentdocs-eu-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agentdocs Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: agentdocs-eu declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: agentdocs-eu
provider_slug: agentdocs-eu
scheme_count: 3
schemes:
- description: 'JWT token, valid 7 days, sent in Authorization: Bearer <jwt>'
  scheme: bearer
  type: http
- description: 'API token, sent as "Authorization: Token <token>"'
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.1 for MCP connectors, automatic refresh
  flows:
    authorizationCode:
      authorizationUrl: https://agentdocs.eu/mcp/authorize
      scopes: {}
      tokenUrl: https://agentdocs.eu/mcp/token
  type: oauth2
slug: agentdocs-eu-authentication
source_filename: agentdocs-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://agentdocs.eu/docs/api-auth\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"JWT token, valid 7 days, sent in Authorization: Bearer <jwt>\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"API token, sent as \\\"Authorization: Token <token>\\\"\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://agentdocs.eu/mcp/authorize\n        tokenUrl: https://agentdocs.eu/mcp/token\n        scopes: {}\n    description: \"OAuth 2.1 for MCP connectors, automatic refresh\"\n"
source_yaml_url: https://artifacts.apis.io/agentdocs-eu/authentication/agentdocs-eu-authentication.yml
summary_line: 3 schemes
tags:
- Collaboration
- Documentation
- AI
- Platform
- OpenSource
- Company
---
