---
api_key_in: []
api_specs:
- filename: corridor-openapi.yml
  format: yaml
  label: Corridor API
  slug: corridor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corridor/refs/heads/main/openapi/corridor-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Corridor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corridor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Corridor
provider_slug: corridor
scheme_count: 1
schemes:
- description: 'API token with the `cor_` prefix, generated from Profile > API Tokens in the Corridor dashboard (https://app.corridor.dev/settings). Passed as `Authorization: Bearer [example key]`. Tokens carry the same access as the user who created them but cannot perform admin operations.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/corridor-openapi.yml
  type: http
slug: corridor-authentication
source_filename: corridor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/corridor-openapi.yml\ndocs: https://docs.corridor.dev/api/reference\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_prefix: cor_\n  admin_operations: Require a standard user session; API tokens are rejected for admin operations.\n  sso: SSO via Okta available for enterprise accounts (docs.corridor.dev/administration/sso-okta).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API token with the `cor_` prefix, generated from Profile > API Tokens in the\n    Corridor dashboard (https://app.corridor.dev/settings). Passed as\n    `Authorization: Bearer [example key]`. Tokens carry the same access as the user who\n    created them but cannot perform admin operations.\n  sources:\n  - openapi/corridor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corridor/refs/heads/main/authentication/corridor-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Application Security
- AI Coding
- Code Security
- Developer Tools
- Guardrails
- MCP
- Static Analysis
- DevSecOps
---
