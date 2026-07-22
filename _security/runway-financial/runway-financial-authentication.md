---
api_key_in: []
api_specs:
- filename: runway-financial-export-api-openapi.yml
  format: yaml
  label: Runway Export API
  slug: runway-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway-financial/refs/heads/main/openapi/runway-financial-export-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runway Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runway Financial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runway Financial
provider_slug: runway-financial
scheme_count: 1
schemes:
- description: 'Bearer token using an API secret generated in the Runway app under Settings > API. Pass it as `Authorization: Bearer <your API secret>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runway-financial-export-api-openapi.yml
  type: http
slug: runway-financial-authentication
source_filename: runway-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/runway-financial-export-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token using an API secret generated in the Runway app under Settings\n    > API. Pass it as `Authorization: Bearer <your API secret>`.'\n  sources:\n  - openapi/runway-financial-export-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway-financial/refs/heads/main/authentication/runway-financial-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial Planning
- FP&A
- Forecasting
- Budgeting
- Finance
- MCP
- Export API
- SaaS
---
