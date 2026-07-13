---
api_key_in: []
api_specs:
- filename: quickbooks-accounting.yml
  format: yaml
  label: QuickBooks Online Accounting API
  slug: quickbooks-accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/openapi/quickbooks-accounting.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Intuit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Intuit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Intuit
provider_slug: intuit
scheme_count: 1
schemes:
- description: Intuit uses OAuth 2.0 for authorization. Apps must be registered on the Intuit Developer portal to obtain client credentials. Access tokens have a 60-minute lifetime and can be refreshed using refresh tokens (100-day lifetime).
  flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: oauth2
  sources:
  - openapi/quickbooks-accounting.yml
  type: oauth2
slug: intuit-authentication
source_filename: intuit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quickbooks-accounting.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n    scopes: 1\n  description: Intuit uses OAuth 2.0 for authorization. Apps must be registered on the Intuit\n    Developer portal to obtain client credentials. Access tokens have a 60-minute lifetime and\n    can be refreshed using refresh tokens (100-day lifetime).\n  sources:\n  - openapi/quickbooks-accounting.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/authentication/intuit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
- Fortune 1000
---
