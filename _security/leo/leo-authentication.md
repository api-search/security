---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leo-prospects-api-openapi.yml
  format: yaml
  label: LeO Public API
  slug: leo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-prospects-api-openapi.yml
- filename: leo-health-api-openapi.yml
  format: yaml
  label: LeO Health API
  slug: leo-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-health-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Leo Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LeO
provider_slug: leo
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/leo-account-api-openapi.yml
  - openapi/leo-credits-api-openapi.yml
  - openapi/leo-health-api-openapi.yml
  - openapi/leo-jobs-api-openapi.yml
  - openapi/leo-prospects-api-openapi.yml
  type: http
slug: leo-authentication
source_filename: leo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/leo-account-api-openapi.yml, openapi/leo-credits-api-openapi.yml, openapi/leo-health-api-openapi.yml,\n  openapi/leo-jobs-api-openapi.yml, openapi/leo-prospects-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/leo-account-api-openapi.yml\n  - openapi/leo-credits-api-openapi.yml\n  - openapi/leo-health-api-openapi.yml\n  - openapi/leo-jobs-api-openapi.yml\n  - openapi/leo-prospects-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/authentication/leo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
- Data Enrichment
- Sales Intelligence
- Non-Profit
- Trucking
- MCP
- Agent-Native
---
