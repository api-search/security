---
api_key_in: []
api_specs:
- filename: brex-budget-programs-api-openapi.yml
  format: yaml
  label: Brex Budget Programs API
  slug: brex-budget-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brex/refs/heads/main/openapi/brex-budget-programs-api-openapi.yml
- filename: brex-budgets-api-openapi.yml
  format: yaml
  label: Brex Budgets API
  slug: brex-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brex/refs/heads/main/openapi/brex-budgets-api-openapi.yml
- filename: brex-spend-limits-api-openapi.yml
  format: yaml
  label: Brex Spend Limits API
  slug: brex-spend-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brex/refs/heads/main/openapi/brex-spend-limits-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brex
provider_slug: brex
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/brex-openapi.yml
  type: http
slug: brex-authentication
source_filename: brex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brex-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/brex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brex/refs/heads/main/authentication/brex-authentication.yml
summary_line: http · 1 scheme
tags:
- Bill Pay
- Corporate Cards
- Expenses
- Reimbursements
- Spending
---
