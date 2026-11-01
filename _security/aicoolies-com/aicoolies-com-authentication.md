---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aicoolies Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: aicoolies declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: aicoolies
provider_slug: aicoolies-com
scheme_count: 2
schemes:
- authorizationUrl: https://github.com/login/oauth/authorize
  description: GitHub OAuth for human sign‑in; only read:user and user:email scopes are requested.
  flow: authorizationCode
  scopes:
  - read:user
  - user:email
  tokenUrl: https://github.com/login/oauth/access_token
  type: oauth2
- description: Public catalog reads are unauthenticated (CORS *)
  type: none
slug: aicoolies-com-authentication
source_filename: aicoolies-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://aicoolies.com/developers.md\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://github.com/login/oauth/authorize\n    tokenUrl: https://github.com/login/oauth/access_token\n    scopes:\n      - read:user\n      - user:email\n    description: \"GitHub OAuth for human sign‑in; only read:user and user:email scopes are requested.\"\n  - type: none\n    description: \"Public catalog reads are unauthenticated (CORS *)\"\n"
source_yaml_url: https://artifacts.apis.io/aicoolies-com/authentication/aicoolies-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Developer Tools
- Directory
- Reviews
- Comparisons
---
