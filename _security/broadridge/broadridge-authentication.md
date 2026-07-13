---
api_key_in: []
api_specs:
- filename: broadridge-wealth-openapi.yml
  format: yaml
  label: Broadridge Wealth Management API
  slug: broadridge-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/openapi/broadridge-wealth-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Broadridge Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: broadridge secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: broadridge
provider_slug: broadridge
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://auth.broadridge.example.com/oauth/token
  name: oauth2
  sources:
  - openapi/broadridge-wealth-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/broadridge-wealth-openapi.yml
  type: http
slug: broadridge-authentication
source_filename: broadridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/broadridge-wealth-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.broadridge.example.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/broadridge-wealth-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/broadridge-wealth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/authentication/broadridge-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fortune 1000
---
