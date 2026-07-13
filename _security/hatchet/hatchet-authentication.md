---
api_key_in:
- cookie
api_specs:
- filename: hatchet-openapi.yml
  format: yaml
  label: Hatchet API
  slug: hatchet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatchet/refs/heads/main/openapi/hatchet-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hatchet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hatchet secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hatchet
provider_slug: hatchet
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hatchet-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: hatchet
  sources:
  - openapi/hatchet-openapi.yml
  type: apiKey
slug: hatchet-authentication
source_filename: hatchet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hatchet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hatchet-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: hatchet\n  sources:\n  - openapi/hatchet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatchet/refs/heads/main/authentication/hatchet-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Task Queue
- Workflow Engine
- Durable Execution
- Background Tasks
- AI Agents
- Orchestration
- PostgreSQL
- Open Source
---
