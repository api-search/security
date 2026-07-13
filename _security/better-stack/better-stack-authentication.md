---
api_key_in: []
api_specs:
- filename: better-stack-openapi.yml
  format: yaml
  label: Better Stack API
  slug: better-stack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Better Stack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Better Stack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Better Stack
provider_slug: better-stack
scheme_count: 1
schemes:
- description: Bearer token authentication. Use a global API token or a team-scoped Uptime API token obtained from Better Stack Settings → API tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/better-stack-openapi.yml
  type: http
slug: better-stack-authentication
source_filename: better-stack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/better-stack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Use a global API token or a team-scoped Uptime API\n    token obtained from Better Stack Settings → API tokens.\n  sources:\n  - openapi/better-stack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/authentication/better-stack-authentication.yml
summary_line: http · 1 scheme
tags:
- Incidents
- Logs
- Monitoring
- Platform
- Status
- Uptime
- Observability
- On-Call
- Heartbeats
---
