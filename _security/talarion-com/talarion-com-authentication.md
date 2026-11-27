---
anonymous_access: false
api_key_in: []
api_specs:
- filename: talarion-com-fetch-api-openapi.yml
  format: yaml
  label: Talarion Fetch API
  slug: talarion-com-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talarion-com/openapi/talarion-com-fetch-api-openapi.yml
- filename: talarion-com-research-api-openapi.yml
  format: yaml
  label: Talarion Research API
  slug: talarion-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talarion-com/openapi/talarion-com-research-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Talarion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talarion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Talarion
provider_slug: talarion-com
scheme_count: 2
schemes:
- description: OAuth flow for MCP clients with dynamic client registration.
  flows:
    authorizationCode:
      authorizationUrl: https://dashboard.talarion.com/oauth/authorize
      scopes: {}
      tokenUrl: https://dashboard.talarion.com/oauth/token
  type: oauth2
- description: Workspace-scoped API keys used as Bearer token.
  in: header
  name: Authorization
  type: apiKey
slug: talarion-com-authentication
source_filename: talarion-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: searched\nsource: https://docs.talarion.com/authentication.md\nschemes:\n  - type: oauth2\n    description: OAuth flow for MCP clients with dynamic client registration.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://dashboard.talarion.com/oauth/authorize\n        tokenUrl: https://dashboard.talarion.com/oauth/token\n        scopes: {}\n  - type: apiKey\n    description: Workspace-scoped API keys used as Bearer token.\n    name: Authorization\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/talarion-com/authentication/talarion-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Search
- KnowledgeBase
- LLM
- API
---
