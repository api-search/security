---
api_key_in: []
api_specs:
- filename: paychex-payroll-companies-openapi.yml
  format: yaml
  label: Paychex Payroll Companies API
  slug: paychex-payroll-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-payroll-companies-openapi.yml
- filename: paychex-workers-openapi.yml
  format: yaml
  label: Paychex Workers API
  slug: paychex-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-workers-openapi.yml
- filename: paychex-time-openapi.yml
  format: yaml
  label: Paychex Time API
  slug: paychex-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-time-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paychex Developer Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paychex secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paychex
provider_slug: paychex-developer
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  sources:
  - openapi/paychex-payroll-companies-openapi.yml
  - openapi/paychex-time-openapi.yml
  - openapi/paychex-workers-openapi.yml
  type: oauth2
slug: paychex-developer-authentication
source_filename: paychex-developer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paychex-payroll-companies-openapi.yml, openapi/paychex-time-openapi.yml, openapi/paychex-workers-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\n    scopes: 0\n  sources:\n  - openapi/paychex-payroll-companies-openapi.yml\n  - openapi/paychex-time-openapi.yml\n  - openapi/paychex-workers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/authentication/paychex-developer-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Benefits
- HCM
- HR
- Paychex Flex
- Payroll
- Time and Attendance
- Workforce
- Fortune 1000
---
