---
api_key_in:
- header
api_specs:
- filename: mosaic-app-members-api-openapi.yml
  format: yaml
  label: Mosaic Members API
  slug: mosaic-app-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-members-api-openapi.yml
- filename: mosaic-app-projects-api-openapi.yml
  format: yaml
  label: Mosaic Projects API
  slug: mosaic-app-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-projects-api-openapi.yml
- filename: mosaic-app-tasks-api-openapi.yml
  format: yaml
  label: Mosaic Tasks API
  slug: mosaic-app-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-tasks-api-openapi.yml
- filename: mosaic-app-time-entries-api-openapi.yml
  format: yaml
  label: Mosaic Time Entries API
  slug: mosaic-app-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-time-entries-api-openapi.yml
- filename: mosaic-app-work-plans-api-openapi.yml
  format: yaml
  label: Mosaic Work Plans API
  slug: mosaic-app-work-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-work-plans-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mosaic App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mosaic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mosaic
provider_slug: mosaic-app
scheme_count: 1
schemes:
- description: 'API token issued by your Mosaic Customer Success Manager. Send as the

    raw `Authorization` header value (no `Bearer` prefix).'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/mosaic-app-openapi.yml
  type: apiKey
slug: mosaic-app-authentication
source_filename: mosaic-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mosaic-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    API token issued by your Mosaic Customer Success Manager. Send as the\n    raw `Authorization` header value (no `Bearer` prefix).\n  sources:\n  - openapi/mosaic-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/authentication/mosaic-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Resource Management
- Workforce Planning
- Project Management
- AEC
- Professional Services
- Time Tracking
- Forecasting
- AI Assistant
- Integration Platform
- Fortune 500
---
