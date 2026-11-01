---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Team0 Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: team0-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: team0-ai
provider_slug: team0-ai
scheme_count: 2
schemes:
- bearerFormat: Team0 API key
  description: 'Server-only Authorization: Bearer t0_live_... token'
  scheme: bearer
  type: http
- description: Delegated-human OAuth issued by Clerk
  flows:
    authorizationCode:
      authorizationUrl: https://clerk.team0.ai/oauth/authorize
      scopes: []
      tokenUrl: https://clerk.team0.ai/oauth/token
  type: oauth2
slug: team0-ai-authentication
source_filename: team0-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://team0.ai/developers.md\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: \"Team0 API key\"\n    description: \"Server-only Authorization: Bearer t0_live_... token\"\n  - type: oauth2\n    description: \"Delegated-human OAuth issued by Clerk\"\n    flows:\n      authorizationCode:\n        authorizationUrl: https://clerk.team0.ai/oauth/authorize\n        tokenUrl: https://clerk.team0.ai/oauth/token\n        scopes: []\n"
source_yaml_url: https://artifacts.apis.io/team0-ai/authentication/team0-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Enterprise
- KnowledgeManagement
- Automation
---
