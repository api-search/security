---
api_key_in:
- header
api_specs:
- filename: wagestream-absences-api-openapi.yml
  format: yaml
  label: Wagestream Absences API
  slug: wagestream-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-absences-api-openapi.yml
- filename: wagestream-employees-api-openapi.yml
  format: yaml
  label: Wagestream Employees API
  slug: wagestream-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-employees-api-openapi.yml
- filename: wagestream-enrollment-api-openapi.yml
  format: yaml
  label: Wagestream Enrollment API
  slug: wagestream-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-enrollment-api-openapi.yml
- filename: wagestream-off-cycle-payment-api-openapi.yml
  format: yaml
  label: Wagestream Off Cycle Payment API
  slug: wagestream-off-cycle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-off-cycle-payment-api-openapi.yml
- filename: wagestream-shifts-api-openapi.yml
  format: yaml
  label: Wagestream Shifts API
  slug: wagestream-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-shifts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wagestream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wagestream secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wagestream
provider_slug: wagestream
scheme_count: 1
schemes:
- in: header
  name: name
  parameter: x-api-key
  sources:
  - openapi/wagestream-integrations-api-openapi.yml
  type: apiKey
slug: wagestream-authentication
source_filename: wagestream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/wagestream-integrations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: name\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/wagestream-integrations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/authentication/wagestream-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Wellbeing
- Earned Wage Access
- Fintech
- Payroll
- Human Resources
- Workforce Management
- Time and Attendance
- Employee Benefits
- Workplace Savings
- HR Integrations
- B Corp
- United Kingdom
---
