---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Timely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Timely (Memory AS) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Timely (Memory AS)
provider_slug: timely
scheme_count: 2
schemes:
- description: This API uses OAuth 2.0 for authentication.
  flows:
    authorizationCode:
      authorizationUrl: http://api.timelyapp.local:3002/1.1/oauth/authorize
      scopes:
        manage: Grants access
      tokenUrl: http://api.timelyapp.local:3002/1.1/oauth/token
  type: oauth2
- description: Bearer token authentication. Tokens can be obtained via OAuth2 or from the docs login.
  scheme: bearer
  type: http
slug: timely-authentication
source_filename: timely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://developer.timely.com/\nschemes:\n  - type: oauth2\n    description: This API uses OAuth 2.0 for authentication.\n    flows:\n      authorizationCode:\n        authorizationUrl: http://api.timelyapp.local:3002/1.1/oauth/authorize\n        tokenUrl: http://api.timelyapp.local:3002/1.1/oauth/token\n        scopes:\n          manage: Grants access\n  - type: http\n    scheme: bearer\n    description: Bearer token authentication. Tokens can be obtained via OAuth2 or from the docs login.\n"
source_yaml_url: https://artifacts.apis.io/timely/authentication/timely-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Time Tracking
- AI
- SaaS
- Productivity
---
