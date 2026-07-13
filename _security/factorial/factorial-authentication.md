---
api_key_in: []
api_specs:
- filename: factorial-openapi.yml
  format: yaml
  label: Factorial Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/openapi/factorial-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Factorial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Factorial secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Factorial
provider_slug: factorial
scheme_count: 2
schemes:
- description: API key issued from the Factorial settings panel.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/factorial-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.factorialhr.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.factorialhr.com/oauth/token
  name: OAuth2
  sources:
  - openapi/factorial-openapi.yml
  type: oauth2
slug: factorial-authentication
source_filename: factorial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/factorial-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: API key issued from the Factorial settings panel.\n  sources:\n  - openapi/factorial-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.factorialhr.com/oauth/authorize\n    tokenUrl: https://api.factorialhr.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/factorial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/authentication/factorial-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Human Resources
- HRIS
- Employee Management
- Time Tracking
- Payroll
- Time Off
- Performance Management
---
