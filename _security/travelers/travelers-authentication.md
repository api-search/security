---
api_key_in: []
api_specs:
- filename: travelers-openapi.yml
  format: yaml
  label: Travelers API
  slug: travelers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/openapi/travelers-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Travelers Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Travelers secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Travelers
provider_slug: travelers
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.travelers.com/oauth/token
  name: OAuth2
  sources:
  - openapi/travelers-openapi.yml
  type: oauth2
slug: travelers-authentication
source_filename: travelers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travelers-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.travelers.com/oauth/token\n    scopes: 5\n  sources:\n  - openapi/travelers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/authentication/travelers-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Insurance
- Property Casualty
- Commercial Insurance
- Claims
- Fintech
- Fortune 500
---
