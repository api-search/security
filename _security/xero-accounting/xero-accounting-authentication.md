---
api_key_in: []
api_specs:
- filename: Xero-OpenAPI
  format: yaml
  label: Xero Accounting API
  slug: api
  spec_type: OpenAPI
  url: https://github.com/XeroAPI/Xero-OpenAPI
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xero Accounting Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Xero Accounting secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Xero Accounting
provider_slug: xero-accounting
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  sources:
  - openapi/xero-accounting-openapi.yml
  type: oauth2
slug: xero-accounting-authentication
source_filename: xero-accounting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xero-accounting-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n    scopes: 6\n  sources:\n  - openapi/xero-accounting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/authentication/xero-accounting-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Financial Reporting
- SaaS
---
