---
api_key_in: []
api_specs:
- filename: superlog-management-openapi.json
  format: json
  label: Superlog Management API
  slug: superlog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/openapi/superlog-management-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Superlog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superlog secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Superlog
provider_slug: superlog
scheme_count: 1
schemes:
- bearerFormat: sl_management_*
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/superlog-management-openapi.json
  type: http
slug: superlog-authentication
source_filename: superlog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/superlog-management-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sl_management_*\n  sources:\n  - openapi/superlog-management-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/authentication/superlog-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Observability
- OpenTelemetry
- Monitoring
- Logging
- Tracing
- Metrics
- Incident Management
- AI Agents
- Model Context Protocol
- Developer Tools
---
