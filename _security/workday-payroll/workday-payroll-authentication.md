---
api_key_in: []
api_specs:
- filename: workday-payroll-payroll-openapi.yml
  format: yaml
  label: Workday Payroll API
  slug: workday-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/openapi/workday-payroll-payroll-openapi.yml
- filename: workday-payroll-payroll-results-openapi.yml
  format: yaml
  label: Workday Payroll Results API
  slug: workday-payroll-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/openapi/workday-payroll-payroll-results-openapi.yml
- filename: workday-payroll-payroll-input-openapi.yml
  format: yaml
  label: Workday Payroll Input API
  slug: workday-payroll-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/openapi/workday-payroll-payroll-input-openapi.yml
- filename: workday-payroll-tax-openapi.yml
  format: yaml
  label: Workday Tax API
  slug: workday-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/openapi/workday-payroll-tax-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Payroll Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Payroll secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workday Payroll
provider_slug: workday-payroll
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained through Workday authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-payroll-payroll-input-openapi.yml
  - openapi/workday-payroll-payroll-openapi.yml
  - openapi/workday-payroll-payroll-results-openapi.yml
  - openapi/workday-payroll-tax-openapi.yml
  type: http
slug: workday-payroll-authentication
source_filename: workday-payroll-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-payroll-payroll-input-openapi.yml, openapi/workday-payroll-payroll-openapi.yml,\n  openapi/workday-payroll-payroll-results-openapi.yml, openapi/workday-payroll-tax-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained through Workday authentication.\n  sources:\n  - openapi/workday-payroll-payroll-input-openapi.yml\n  - openapi/workday-payroll-payroll-openapi.yml\n  - openapi/workday-payroll-payroll-results-openapi.yml\n  - openapi/workday-payroll-tax-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/authentication/workday-payroll-authentication.yml
summary_line: http · 1 scheme
tags:
- Compensation
- Enterprise
- Human Resources
- Payroll
- SaaS
- Tax
---
