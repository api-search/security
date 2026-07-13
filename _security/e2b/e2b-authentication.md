---
api_key_in:
- header
api_specs:
- filename: e2b-openapi.yml
  format: yaml
  label: E2B Sandbox API
  slug: sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b/refs/heads/main/openapi/e2b-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: E2B Authentication
name_suffix: Authentication
oauth_flows: []
overview: E2B secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: E2B
provider_slug: e2b
scheme_count: 1
schemes:
- in: header
  name: E2BApiKey
  parameter: X-API-Key
  sources:
  - openapi/e2b-openapi.yml
  type: apiKey
slug: e2b-authentication
source_filename: e2b-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/e2b-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: E2BApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/e2b-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2b/refs/heads/main/authentication/e2b-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Code Interpreter
- Sandboxes
- Secure Execution
- AI Agents
- Firecracker
- microVMs
- Code Execution
- Data Analysis
- Desktop Sandbox
- Computer Use
- Custom Templates
- Python
- TypeScript
---
