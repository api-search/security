---
api_key_in: []
api_specs:
- filename: postman-freeagent-api-collection
  format: yaml
  label: FreeAgent REST API
  slug: rest-api
  spec_type: Postman
  url: https://github.com/fac/postman-freeagent-api-collection
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Freeagent Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FreeAgent secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FreeAgent
provider_slug: freeagent
scheme_count: 1
schemes:
- description: 'OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;

    refresh tokens used to obtain new access tokens.'
  flows:
  - authorizationUrl: https://api.freeagent.com/v2/approve_app
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.freeagent.com/v2/token_endpoint
  name: oauth2
  sources:
  - openapi/freeagent-openapi.yml
  type: oauth2
slug: freeagent-authentication
source_filename: freeagent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freeagent-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freeagent.com/v2/approve_app\n    tokenUrl: https://api.freeagent.com/v2/token_endpoint\n    scopes: 0\n  description: |-\n    OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;\n    refresh tokens used to obtain new access tokens.\n  sources:\n  - openapi/freeagent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/authentication/freeagent-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Expenses
- Payroll
- VAT
- HMRC
- Making Tax Digital
---
