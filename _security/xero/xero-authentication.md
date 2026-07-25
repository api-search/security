---
api_key_in: []
api_specs:
- filename: xero-accounting-api-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-api-openapi.yml
- filename: xero-asset-api-openapi.yml
  format: yaml
  label: Xero Asset API
  slug: xero-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-asset-api-openapi.yml
- filename: xero-bankfeeds-api-openapi.yml
  format: yaml
  label: Xero BankFeeds API
  slug: xero-bankfeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bankfeeds-api-openapi.yml
- filename: xero-files-api-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-api-openapi.yml
- filename: xero-finance-api-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-api-openapi.yml
- filename: xero-identity-api-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-api-openapi.yml
- filename: xero-payrollau-api-openapi.yml
  format: yaml
  label: Xero PayrollAu API
  slug: xero-payrollau-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollau-api-openapi.yml
- filename: xero-payrollnz-api-openapi.yml
  format: yaml
  label: Xero PayrollNz API
  slug: xero-payrollnz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollnz-api-openapi.yml
- filename: xero-payrolluk-api-openapi.yml
  format: yaml
  label: Xero PayrollUk API
  slug: xero-payrolluk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrolluk-api-openapi.yml
- filename: xero-project-api-openapi.yml
  format: yaml
  label: Xero Project API
  slug: xero-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-project-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xero Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Xero secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Xero
provider_slug: xero
scheme_count: 2
schemes:
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    scopes: 16
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  sources:
  - openapi/xero-accounting-openapi.yml
  - openapi/xero-assets-openapi.yml
  - openapi/xero-bankfeeds-openapi.yml
  - openapi/xero-files-openapi.yml
  - openapi/xero-finance-openapi.yml
  - openapi/xero-identity-openapi.yml
  - openapi/xero-payroll-au-openapi.yml
  - openapi/xero-payroll-nz-openapi.yml
  - openapi/xero-payroll-uk-openapi.yml
  - openapi/xero-projects-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/xero-identity-openapi.yml
  type: http
slug: xero-authentication
source_filename: xero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xero-accounting-openapi.yml, openapi/xero-assets-openapi.yml, openapi/xero-bankfeeds-openapi.yml,\n  openapi/xero-files-openapi.yml, openapi/xero-finance-openapi.yml, openapi/xero-identity-openapi.yml,\n  openapi/xero-payroll-au-openapi.yml, openapi/xero-payroll-nz-openapi.yml, openapi/xero-payroll-uk-openapi.yml,\n  openapi/xero-projects-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n    scopes: 16\n  description: For more information\n  sources:\n  - openapi/xero-accounting-openapi.yml\n  - openapi/xero-assets-openapi.yml\n  - openapi/xero-bankfeeds-openapi.yml\n  - openapi/xero-files-openapi.yml\n  - openapi/xero-finance-openapi.yml\n  - openapi/xero-identity-openapi.yml\n\
  \  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n  - openapi/xero-projects-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/xero-identity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/authentication/xero-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
---
