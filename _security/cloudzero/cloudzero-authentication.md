---
api_key_in:
- header
api_specs:
- filename: cloudzero-api-openapi.yml
  format: yaml
  label: CloudZero API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudZero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudZero
provider_slug: cloudzero
scheme_count: 1
schemes:
- description: API key for authentication. Include your API key directly in the Authorization header.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/cloudzero-api-openapi.yml
  type: apiKey
slug: cloudzero-authentication
source_filename: cloudzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudzero-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authentication. Include your API key directly in the Authorization\n    header.\n  sources:\n  - openapi/cloudzero-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/authentication/cloudzero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
---
