---
api_key_in: []
api_specs:
- filename: better-stack-escalation-policies-api-openapi.yml
  format: yaml
  label: Better Stack Escalation Policies API
  slug: better-stack-escalation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-escalation-policies-api-openapi.yml
- filename: better-stack-heartbeats-api-openapi.yml
  format: yaml
  label: Better Stack Heartbeats API
  slug: better-stack-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-heartbeats-api-openapi.yml
- filename: better-stack-incidents-api-openapi.yml
  format: yaml
  label: Better Stack Incidents API
  slug: better-stack-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-incidents-api-openapi.yml
- filename: better-stack-monitors-api-openapi.yml
  format: yaml
  label: Better Stack Monitors API
  slug: better-stack-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-monitors-api-openapi.yml
- filename: better-stack-status-pages-api-openapi.yml
  format: yaml
  label: Better Stack Status Pages API
  slug: better-stack-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-status-pages-api-openapi.yml
- filename: better-stack-team-members-api-openapi.yml
  format: yaml
  label: Better Stack Team Members API
  slug: better-stack-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-team-members-api-openapi.yml
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
