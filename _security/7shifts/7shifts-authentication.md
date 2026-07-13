---
api_key_in: []
api_specs:
- filename: 7shifts-openapi.yml
  format: yaml
  label: 7shifts REST API v2
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: 7Shifts Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 7shifts secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 7shifts
provider_slug: 7shifts
scheme_count: 2
schemes:
- description: Access token obtained from /oauth2/token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/7shifts-openapi.yml
  type: http
- description: OAuth 2.0 with client_credentials, password, authorization_code, and refresh_token grant types.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.7shifts.com/oauth2/token
  name: oauth2
  sources:
  - openapi/7shifts-openapi.yml
  type: oauth2
slug: 7shifts-authentication
source_filename: 7shifts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/7shifts-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token obtained from /oauth2/token passed as a Bearer token.\n  sources:\n  - openapi/7shifts-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.7shifts.com/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 with client_credentials, password, authorization_code, and refresh_token\n    grant types.\n  sources:\n  - openapi/7shifts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/authentication/7shifts-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Restaurant
- Scheduling
- Workforce Management
- Employee Scheduling
- Time Tracking
- HRIS
- Labor
---
