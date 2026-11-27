---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DirectCase Authentication
name_suffix: Authentication
oauth_flows: []
overview: DirectCase declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DirectCase
provider_slug: directcase-ai
scheme_count: 1
schemes:
- description: OAuth 2.1 (WorkOS AuthKit) used for MCP connector authentication.
  flows:
    authorizationCode:
      authorizationUrl: https://login.directcase.ai/authorize
      scopes: {}
      tokenUrl: https://login.directcase.ai/token
  type: oauth2
slug: directcase-ai-authentication
source_filename: directcase-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.directcase.ai/gb/en/docs/mcp\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 (WorkOS AuthKit) used for MCP connector authentication.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://login.directcase.ai/authorize\n        tokenUrl: https://login.directcase.ai/token\n        scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/directcase-ai/authentication/directcase-ai-authentication.yml
summary_line: 1 scheme
tags:
- Legal Tech
- Artificial Intelligence
- Research
- Law
- Software-as-a-Service
---
