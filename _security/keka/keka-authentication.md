---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Keka HR REST API
  slug: keka-hr-rest-api
  spec_type: OpenAPI
  url: https://apidocs.keka.com/
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Keka Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Keka HR secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Keka HR
provider_slug: keka
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.keka.com/connect/token
  name: oauth2
  sources:
  - openapi/keka-hr-api-openapi.yaml
  type: oauth2
slug: keka-authentication
source_filename: keka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keka-hr-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.keka.com/connect/token\n    scopes: 1\n  description: OAuth 2.0 client credentials flow\n  sources:\n  - openapi/keka-hr-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/authentication/keka-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- Human Resources
- Payroll
- Attendance
- Leave Management
- Performance Management
- Employee Management
- India
- HRMS
---
