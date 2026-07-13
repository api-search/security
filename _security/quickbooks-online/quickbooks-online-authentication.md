---
api_key_in: []
api_specs:
- filename: openapi-specifications
  format: yaml
  label: QuickBooks Online Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://developer.intuit.com/app/developer/qbo/docs/develop/explore-the-quickbooks-online-api/openapi-specifications
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Quickbooks Online Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: QuickBooks Online secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: QuickBooks Online
provider_slug: quickbooks-online
scheme_count: 1
schemes:
- description: Intuit OAuth 2.0
  flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: OAuth2
  sources:
  - openapi/quickbooks-online-openapi.yml
  type: oauth2
slug: quickbooks-online-authentication
source_filename: quickbooks-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quickbooks-online-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n    scopes: 5\n  description: Intuit OAuth 2.0\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickbooks-online/refs/heads/main/authentication/quickbooks-online-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Bookkeeping
- Invoicing
- Small Business
- Finance
- Payments
- Payroll
---
