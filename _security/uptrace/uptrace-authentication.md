---
api_key_in:
- header
api_specs:
- filename: uptrace-openapi.yml
  format: yaml
  label: Uptrace API
  slug: uptrace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrace/refs/heads/main/openapi/uptrace-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uptrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptrace secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uptrace
provider_slug: uptrace
scheme_count: 2
schemes:
- description: 'DSN-based token: ''Bearer <project_secret_token>'''
  in: header
  name: DSNAuth
  parameter: Authorization
  sources:
  - openapi/uptrace-openapi.yml
  type: apiKey
- description: Uptrace API token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/uptrace-openapi.yml
  type: http
slug: uptrace-authentication
source_filename: uptrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uptrace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: DSNAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'DSN-based token: ''Bearer <project_secret_token>'''\n  sources:\n  - openapi/uptrace-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Uptrace API token\n  sources:\n  - openapi/uptrace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptrace/refs/heads/main/authentication/uptrace-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- APM
- Observability
- OpenTelemetry
- Distributed Tracing
- Monitoring
---
