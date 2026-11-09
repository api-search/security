---
anonymous_access: false
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: 2Pr Io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 2pr secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 2pr
provider_slug: 2pr-io
scheme_count: 2
schemes:
- description: '"Sign in with 2pr". Authorization code with PKCE S256; register a client first.'
  flows:
  - authorizationUrl: https://2pr.io/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://2pr.io/api/oauth/token
  name: oauth2
  sources:
  - openapi/2pr-io-openapi.json
  type: oauth2
- description: Personal token created by the account owner under https://2pr.io/app/preferences. Revocable there at any time.
  name: personalToken
  scheme: bearer
  sources:
  - openapi/2pr-io-openapi.json
  type: http
slug: 2pr-io-authentication
source_filename: 2pr-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/2pr-io-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://2pr.io/oauth/authorize\n    tokenUrl: https://2pr.io/api/oauth/token\n    scopes: 1\n  description: '\"Sign in with 2pr\". Authorization code with PKCE S256; register a client first.'\n  sources:\n  - openapi/2pr-io-openapi.json\n- name: personalToken\n  type: http\n  scheme: bearer\n  description: Personal token created by the account owner under https://2pr.io/app/preferences.\n    Revocable there at any time.\n  sources:\n  - openapi/2pr-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/2pr-io/authentication/2pr-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- LinkedIn
- Marketing
- Automation
- Software-as-a-Service
---
