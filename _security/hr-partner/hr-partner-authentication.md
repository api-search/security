---
api_key_in:
- header
api_specs:
- filename: hr-partner-rest-api-openapi.yml
  format: yaml
  label: HR Partner REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hr-partner/refs/heads/main/openapi/hr-partner-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hr Partner Authentication
name_suffix: Authentication
oauth_flows: []
overview: HR Partner secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HR Partner
provider_slug: hr-partner
scheme_count: 1
schemes:
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/hr-partner-rest-api-openapi.yml
  type: apiKey
slug: hr-partner-authentication
source_filename: hr-partner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hr-partner-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/hr-partner-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hr-partner/refs/heads/main/authentication/hr-partner-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- HR
- HRIS
- Human Resources
- Employee Records
- Leave Management
- Recruitment
- Applicant Tracking
- Onboarding
- Performance Management
- Timesheets
- Expense Management
- Document Library
- eSignature
- SaaS
- Australia
---
