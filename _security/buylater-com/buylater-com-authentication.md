---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Buylater Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuyLater declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BuyLater
provider_slug: buylater-com
scheme_count: 1
schemes:
- authorizationUrl: https://buylater.com/api/oauth/authorize
  description: OAuth 2.1 via Clerk for user authentication.
  flow: authorizationCode
  tokenUrl: https://buylater.com/api/oauth/token
  type: oauth2
slug: buylater-com-authentication
source_filename: buylater-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://buylater.com/docs\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    description: OAuth 2.1 via Clerk for user authentication.\n    tokenUrl: https://buylater.com/api/oauth/token\n    authorizationUrl: https://buylater.com/api/oauth/authorize\n"
source_yaml_url: https://artifacts.apis.io/buylater-com/authentication/buylater-com-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Notification
- AI Assistant
- MCP
- Shopping
---
