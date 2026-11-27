---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arketo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arketo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arketo
provider_slug: arketo-ai
scheme_count: 1
schemes:
- description: OAuth2 login via Google or GitHub
  flows:
    authorizationCode:
      authorizationUrl: https://arketo.ai/api/auth/oauth/google/start
      scopes: []
      tokenUrl: https://arketo.ai/api/auth/oauth/google/callback
  type: oauth2
slug: arketo-ai-authentication
source_filename: arketo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource:\n  - https://arketo.ai/api/auth/oauth/google/start\n  - https://arketo.ai/api/auth/oauth/github/start\nschemes:\n  - type: oauth2\n    description: OAuth2 login via Google or GitHub\n    flows:\n      authorizationCode:\n        authorizationUrl: https://arketo.ai/api/auth/oauth/google/start\n        tokenUrl: https://arketo.ai/api/auth/oauth/google/callback\n        scopes: []\n"
source_yaml_url: https://artifacts.apis.io/arketo-ai/authentication/arketo-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Architecture
- Developer Tools
- LLM
- Software Engineering
---
