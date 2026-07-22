---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Quantive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quantive declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Quantive
provider_slug: quantive
scheme_count: 2
schemes:
- description: Recommended for multi-user applications. Register an app, obtain an authorization code, exchange it for an access token, and pass the token as a bearer credential in the Authorization header. Access tokens are valid for one year.
  endpoints:
    authorization: https://www.myworkboard.com/wb/oauth/authorize
    revocation: https://www.myworkboard.com/wb/oauth/revoke/
    token: https://www.myworkboard.com/wb/oauth/token
  flow: authorization_code
  header: Authorization
  id: oauth2-authorization-code
  in: header
  scopes:
  - all
  token_format: Bearer
  type: oauth2
- description: Instant Token Authentication issues an access token with a single click from the WorkBoard app-management portal. Intended for testing or single-user applications. Passed as a bearer credential in the Authorization header.
  header: Authorization
  id: instant-token
  in: header
  issued_at: https://www.myworkboard.com/wb/user/profile/edit?do=mgApp
  token_format: Bearer
  type: apiKey
slug: quantive-authentication
source_filename: quantive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: 2026-07-20\nmethod: searched\nsource: https://www.workboard.com/developer\napi: WorkBoard REST API (Quantive)\nnotes: >-\n  Quantive (formerly Gtmhub) merged into WorkBoard; the live developer surface is\n  the WorkBoard REST API v1.0. Auth details captured verbatim from the public\n  WorkBoard developer documentation. No OpenAPI specification is published, so this\n  profile is search-derived from the docs rather than spec-derived.\nschemes:\n- id: oauth2-authorization-code\n  type: oauth2\n  flow: authorization_code\n  description: >-\n    Recommended for multi-user applications. Register an app, obtain an\n    authorization code, exchange it for an access token, and pass the token as a\n    bearer credential in the Authorization header. Access tokens are valid for\n    one year.\n  endpoints:\n    authorization: https://www.myworkboard.com/wb/oauth/authorize\n    token: https://www.myworkboard.com/wb/oauth/token\n    revocation: https://www.myworkboard.com/wb/oauth/revoke/\n\
  \  scopes:\n  - all\n  in: header\n  header: Authorization\n  token_format: Bearer\n- id: instant-token\n  type: apiKey\n  description: >-\n    Instant Token Authentication issues an access token with a single click from\n    the WorkBoard app-management portal. Intended for testing or single-user\n    applications. Passed as a bearer credential in the Authorization header.\n  in: header\n  header: Authorization\n  token_format: Bearer\n  issued_at: https://www.myworkboard.com/wb/user/profile/edit?do=mgApp\ntransport:\n  https_required: true\napp_registration: https://www.myworkboard.com/wb/user/profile/edit?do=mgApp\ndocs: https://www.workboard.com/developer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantive/refs/heads/main/authentication/quantive-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Business Applications
- OKR
- Strategy Execution
- Goal Management
- Performance Management
- SaaS
---
