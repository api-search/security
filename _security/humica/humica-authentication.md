---
api_key_in: []
auth_types:
- oauth2
description: Authentication profile for the Employment Hero API (the platform behind humi.ca — Humi is now Employment Hero Canada). The API uses OAuth 2.0 authorization-code with PKCE (S256) mandatory as of 2026-09-14. Bearer access tokens are short-lived (15 minutes); refresh tokens currently do not expire. Token requests are sent as application/x-www-form-urlencoded.
kind: authentication
layout: security
method: searched
name: Humica Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: humi.ca secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: humi.ca
provider_slug: humica
scheme_count: 1
schemes:
- access_token_lifetime: 15 minutes
  authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize
  docs: https://developer.employmenthero.com/api-references
  flow: authorizationCode
  name: OAuth2
  pkce:
    code_challenge_method: S256
    required: true
  refresh_token_lifetime: no expiration (current)
  sources:
  - https://developer.employmenthero.com/api-references
  tokenUrl: https://oauth.employmenthero.com/oauth2/token
  token_type: Bearer
  type: oauth2
slug: humica-authentication
source_filename: humica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.employmenthero.com/api-references\ndescription: >-\n  Authentication profile for the Employment Hero API (the platform behind\n  humi.ca — Humi is now Employment Hero Canada). The API uses OAuth 2.0\n  authorization-code with PKCE (S256) mandatory as of 2026-09-14. Bearer access\n  tokens are short-lived (15 minutes); refresh tokens currently do not expire.\n  Token requests are sent as application/x-www-form-urlencoded.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce_required: true\n  access_token_ttl_seconds: 900\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize\n    tokenUrl: https://oauth.employmenthero.com/oauth2/token\n    token_type: Bearer\n    pkce:\n      required: true\n      code_challenge_method: S256\n    access_token_lifetime: 15 minutes\n    refresh_token_lifetime: no\
  \ expiration (current)\n    docs: https://developer.employmenthero.com/api-references\n    sources: [https://developer.employmenthero.com/api-references]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humica/refs/heads/main/authentication/humica-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Human Resources
- Payroll
- HR Tech
- Benefits
- Applicant Tracking
- Employer of Record
- Canada
- SaaS
---
