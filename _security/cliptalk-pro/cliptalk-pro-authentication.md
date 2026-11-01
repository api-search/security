---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cliptalk Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClipTalk declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClipTalk
provider_slug: cliptalk-pro
scheme_count: 2
schemes:
- description: OAuth 2.1 Authorization Code flow with PKCE. Tokens are JWTs signed by the server.
  flows:
    authorizationCode:
      authorizationUrl: https://www.cliptalk.pro/.well-known/oauth-protected-resource
      scopes: {}
      tokenUrl: https://www.cliptalk.pro/.well-known/oauth-protected-resource
  type: oauth2
- description: Owner key provided via Authorization header for server-to-server access.
  in: header
  name: Authorization
  type: apiKey
slug: cliptalk-pro-authentication
source_filename: cliptalk-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://www.cliptalk.pro/api/v1\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 Authorization Code flow with PKCE. Tokens are JWTs signed by the server.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.cliptalk.pro/.well-known/oauth-protected-resource\n        tokenUrl: https://www.cliptalk.pro/.well-known/oauth-protected-resource\n        scopes: {}\n  - type: apiKey\n    description: Owner key provided via Authorization header for server-to-server access.\n    name: Authorization\n    in: header"
source_yaml_url: https://artifacts.apis.io/cliptalk-pro/authentication/cliptalk-pro-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Video
- Social Media
- Automation
---
