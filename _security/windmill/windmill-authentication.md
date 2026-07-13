---
api_key_in:
- cookie
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Windmill API
  slug: windmill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/windmill-labs/windmill/main/backend/windmill-api/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Windmill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windmill secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Windmill
provider_slug: windmill
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/windmill-api-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: token
  sources:
  - openapi/windmill-api-openapi.yml
  type: apiKey
slug: windmill-authentication
source_filename: windmill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windmill-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/windmill-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: token\n  sources:\n  - openapi/windmill-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windmill/refs/heads/main/authentication/windmill-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Automation
- Internal Tools
- Open Source
- ProCode API Composition
- Scripts
- Webhooks
- Workflow Engine
- Workflows
---
