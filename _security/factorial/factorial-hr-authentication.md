---
api_key_in:
- header
api_specs:
- filename: factorial-openapi.yml
  format: yaml
  label: Factorial Core Employees API
  slug: factorial-core-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/openapi/factorial-openapi.yml
- filename: factorial-openapi.yml
  format: yaml
  label: Factorial Custom Fields API
  slug: factorial-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/openapi/factorial-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Factorial Hr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Factorial secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Factorial
provider_slug: factorial
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /oauth/token
  name: oauth2
  sources:
  - openapi/factorial-openapi.yml
  type: oauth2
- in: header
  name: apikey
  parameter: x-api-key
  sources:
  - openapi/factorial-openapi.yml
  type: apiKey
slug: factorial-hr-authentication
source_filename: factorial-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/factorial-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 2\n  sources:\n  - openapi/factorial-openapi.yml\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/factorial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/authentication/factorial-hr-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- HR
- Human Resources
- Payroll
- Time Off
- Time Tracking
- ATS
- Performance
- Finance
- Expenses
- Spain
- Barcelona
- All-in-One
---
