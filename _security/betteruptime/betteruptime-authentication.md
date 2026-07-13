---
api_key_in: []
api_specs:
- filename: betteruptime-uptime-api-openapi.yml
  format: yaml
  label: Better Stack Uptime API
  slug: uptime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betteruptime/refs/heads/main/openapi/betteruptime-uptime-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Betteruptime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Better Uptime secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Better Uptime
provider_slug: betteruptime
scheme_count: 1
schemes:
- description: Bearer token obtained from Better Stack account settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/betteruptime-uptime-api-openapi.yml
  type: http
slug: betteruptime-authentication
source_filename: betteruptime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/betteruptime-uptime-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from Better Stack account settings\n  sources:\n  - openapi/betteruptime-uptime-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betteruptime/refs/heads/main/authentication/betteruptime-authentication.yml
summary_line: http · 1 scheme
tags:
- Uptime Monitoring
- Incident Management
- Status Pages
- On-Call Scheduling
- Observability
- DevOps
---
