---
anonymous_access: false
api_key_in: []
api_specs:
- filename: algovesta-com-openapi-generated.yml
  format: yaml
  label: AlgoVesta API
  slug: algovesta-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algovesta-com/openapi/_ae-authored/algovesta-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AlgoVesta Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlgoVesta declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AlgoVesta
provider_slug: algovesta-com
scheme_count: 2
schemes:
- authorizationUrl: https://api.algovesta.com/mcp/oauth/authorize
  description: OAuth 2.1 with PKCE
  scopes: {}
  tokenUrl: https://api.algovesta.com/mcp/oauth/token
  type: oauth2
- description: Secret-link authentication via URL key
  type: secret-link
slug: algovesta-com-authentication
source_filename: algovesta-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://algovesta.com/mcp-docs.html\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 with PKCE\n    authorizationUrl: https://api.algovesta.com/mcp/oauth/authorize\n    tokenUrl: https://api.algovesta.com/mcp/oauth/token\n    scopes: {}\n  - type: secret-link\n    description: Secret-link authentication via URL key\n"
source_yaml_url: https://artifacts.apis.io/algovesta-com/authentication/algovesta-com-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- Trading
- Automation
- Cryptocurrency
- Software-as-a-Service
---
