---
api_key_in: []
api_specs:
- filename: better-stack-openapi.yml
  format: yaml
  label: Better Stack API
  slug: betterstack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Betterstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Better Stack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Better Stack
provider_slug: betterstack
scheme_count: 1
schemes:
- description: 'Bearer token. Provide either a Global API Token (account-wide) or a

    team-scoped Uptime API Token. Issued from Better Stack → API tokens.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/betterstack-openapi.yml
  type: http
slug: betterstack-authentication
source_filename: betterstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/betterstack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token. Provide either a Global API Token (account-wide) or a\n    team-scoped Uptime API Token. Issued from Better Stack → API tokens.\n  sources:\n  - openapi/betterstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/authentication/betterstack-authentication.yml
summary_line: http · 1 scheme
tags:
- Observability
- Uptime Monitoring
- Incidents
- Logs
- Monitoring
- Status Pages
- On-Call
---
