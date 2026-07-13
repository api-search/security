---
api_key_in:
- header
api_specs:
- filename: mosaic-app-openapi.yml
  format: yaml
  label: Mosaic Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-openapi.yml
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
