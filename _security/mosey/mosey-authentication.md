---
api_key_in: []
api_specs:
- filename: mosey-openapi.json
  format: json
  label: Mosey API
  slug: mosey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mosey Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Mosey secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Mosey
provider_slug: mosey
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/mosey-openapi.json
  - openapi/mosey-openapi_v1.json
  - openapi/mosey-openapi_v2.json
  type: oauth2
slug: mosey-authentication
source_filename: mosey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mosey-openapi.json, openapi/mosey-openapi_v1.json, openapi/mosey-openapi_v2.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/token\n    scopes: 0\n  sources:\n  - openapi/mosey-openapi.json\n  - openapi/mosey-openapi_v1.json\n  - openapi/mosey-openapi_v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/authentication/mosey-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Compliance
- Regulatory Technology
- State Compliance
- Tax
- Payroll
- HR
- Business Operations
---
