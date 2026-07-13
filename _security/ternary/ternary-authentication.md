---
api_key_in:
- header
api_specs:
- filename: ternary-openapi.yml
  format: yaml
  label: Ternary API
  slug: ternary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ternary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ternary secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ternary
provider_slug: ternary
scheme_count: 1
schemes:
- description: API key generated from the Ternary platform settings
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/ternary-openapi.yml
  type: apiKey
slug: ternary-authentication
source_filename: ternary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ternary-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key generated from the Ternary platform settings\n  sources:\n  - openapi/ternary-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/authentication/ternary-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Cost Management
- Cost Optimization
- FinOps
- Google Cloud
- Kubernetes
- Multi-Cloud
---
