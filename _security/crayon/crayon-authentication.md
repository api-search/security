---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Crayon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Crayon secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Crayon
provider_slug: crayon
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.crayon.com/api/v1/connect/token
  name: OAuth2
  sources:
  - openapi/crayon-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crayon-openapi.yml
  type: http
slug: crayon-authentication
source_filename: crayon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crayon-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.crayon.com/api/v1/connect/token\n    scopes: 0\n  sources:\n  - openapi/crayon-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/crayon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/authentication/crayon-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- AI
- MCP
---
