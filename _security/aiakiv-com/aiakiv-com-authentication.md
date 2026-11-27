---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AiAkiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: AiAkiv declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AiAkiv
provider_slug: aiakiv-com
scheme_count: 2
schemes:
- description: OAuth flow for user authentication
  flows:
    authorizationCode:
      authorizationUrl: https://app.aiakiv.com/oauth/authorize
      tokenUrl: https://app.aiakiv.com/oauth/token
  type: oauth2
- description: API key authentication for direct access
  in: header
  name: X-API-Key
  type: apiKey
slug: aiakiv-com-authentication
source_filename: aiakiv-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://www.aiakiv.com/docs/en/auth.md\nschemes:\n  - type: oauth2\n    description: OAuth flow for user authentication\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.aiakiv.com/oauth/authorize\n        tokenUrl: https://app.aiakiv.com/oauth/token\n  - type: apiKey\n    description: API key authentication for direct access\n    name: X-API-Key\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/aiakiv-com/authentication/aiakiv-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Knowledge Management
- Team Collaboration
- Memory
- RAG
---
