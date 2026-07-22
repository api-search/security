---
api_key_in:
- header
api_specs:
- filename: process-street-openapi-original.json
  format: json
  label: Process Street Public API
  slug: process-street-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/process-street/refs/heads/main/openapi/process-street-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Process Street Authentication
name_suffix: Authentication
oauth_flows: []
overview: Process Street secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Process Street
provider_slug: process-street
scheme_count: 2
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/process-street-openapi-original.json
  type: apiKey
- description: Bearer token (beta)
  name: httpAuth
  scheme: bearer
  sources:
  - openapi/process-street-openapi-original.json
  type: http
slug: process-street-authentication
source_filename: process-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/process-street-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/process-street-openapi-original.json\n- name: httpAuth\n  type: http\n  scheme: bearer\n  description: Bearer token (beta)\n  sources:\n  - openapi/process-street-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/process-street/refs/heads/main/authentication/process-street-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Productivity
- Workflow
- Workflow Automation
- Process Management
- No-Code
- Business Process
- Task Management
- SaaS
- MCP
---
