---
api_key_in: []
api_specs:
- filename: sage-accounting-openapi.yml
  format: yaml
  label: Sage Accounting API
  slug: accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-accounting-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sage Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sage secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sage
provider_slug: sage
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.sageone.com/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth.accounting.sage.com/token
  name: OAuth2
  sources:
  - openapi/sage-accounting-openapi.yml
  type: oauth2
slug: sage-authentication
source_filename: sage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sage-accounting-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.sageone.com/oauth2/auth\n    tokenUrl: https://oauth.accounting.sage.com/token\n    scopes: 2\n  sources:\n  - openapi/sage-accounting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/authentication/sage-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
---
