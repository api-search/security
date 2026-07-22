---
api_key_in: []
api_specs:
- filename: parsec-teams-openapi.yml
  format: yaml
  label: Parsec for Teams API
  slug: parsec-for-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-teams-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Parsec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parsec secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parsec
provider_slug: parsec
scheme_count: 1
schemes:
- description: 'A Parsec for Teams API key presented as an HTTP Bearer token: `Authorization: Bearer YOUR_API_KEY`. API keys are created and managed in the Parsec for Teams dashboard.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parsec-teams-openapi.yml
  type: http
slug: parsec-authentication
source_filename: parsec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/parsec-teams-openapi.yml\ndocs: https://parsec.app/docs/teams-api\nnotes: >-\n  Parsec for Teams authenticates with an API key presented as an HTTP Bearer\n  token (Authorization: Bearer YOUR_API_KEY). API keys are created and managed\n  in the Parsec for Teams dashboard (dash.parsec.app) and are scoped by a\n  granular team permission model (e.g. View Team Members, Delete Team Machine,\n  Access Audit Log) rather than OAuth scopes.\nsummary:\n  types:\n  - http\n  api_key_style: bearer-token\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Parsec for Teams API key presented as an HTTP Bearer token: `Authorization:\n    Bearer YOUR_API_KEY`. API keys are created and managed in the Parsec for Teams dashboard.'\n  sources:\n  - openapi/parsec-teams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/authentication/parsec-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Remote Desktop
- Cloud Gaming
- Streaming
- Virtual Desktop
- Team Management
- Developer Tools
- Gaming
---
