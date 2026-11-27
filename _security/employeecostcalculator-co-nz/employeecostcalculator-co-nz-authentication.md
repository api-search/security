---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Employee Cost Calculator NZ Authentication
name_suffix: Authentication
oauth_flows: []
overview: Employee Cost Calculator NZ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Employee Cost Calculator NZ
provider_slug: employeecostcalculator-co-nz
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/employeecostcalculator-co-nz-openapi.yml
  type: http
slug: employeecostcalculator-co-nz-authentication
source_filename: employeecostcalculator-co-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/employeecostcalculator-co-nz-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/employeecostcalculator-co-nz-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/employeecostcalculator-co-nz/authentication/employeecostcalculator-co-nz-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payroll
- New Zealand
- Employee Costs
- Calculator
---
