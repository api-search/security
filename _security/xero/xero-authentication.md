---
anonymous_access: false
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
- filename: xero-accountdata-api-openapi.yml
  format: yaml
  label: Xero Account Data API
  slug: xero-accountdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accountdata-api-openapi.yml
- filename: xero-feedconnections-api-openapi.yml
  format: yaml
  label: Xero Feed Connections API
  slug: xero-feedconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-feedconnections-api-openapi.yml
- filename: xero-app-store-api-openapi.yml
  format: yaml
  label: Xero App Store API
  slug: xero-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-app-store-api-openapi.yml
- filename: xero-bank-feeds-api-openapi.yml
  format: yaml
  label: Xero Bank Feeds API
  slug: xero-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bank-feeds-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Xero Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Xero secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Xero
provider_slug: xero
scheme_count: 3
schemes:
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  sources:
  - openapi/xero-account-data-api-openapi.yml
  - openapi/xero-accounting-api-openapi.yml
  - openapi/xero-asset-api-openapi.yml
  - openapi/xero-bank-feeds-api-openapi.yml
  - openapi/xero-bank-feeds-v2-api-openapi.yml
  - openapi/xero-files-api-openapi.yml
  - openapi/xero-finance-api-openapi.yml
  - openapi/xero-identity-api-openapi.yml
  - openapi/xero-payrollau-api-openapi.yml
  - openapi/xero-payrollau-v2-api-openapi.yml
  - openapi/xero-payrollnz-api-openapi.yml
  - openapi/xero-payrolluk-api-openapi.yml
  - openapi/xero-project-api-openapi.yml
  type: oauth2
- description: For more information
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  sources:
  - openapi/xero-app-store-api-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/xero-identity-api-openapi.yml
  type: http
slug: xero-authentication
source_filename: xero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: openapi/xero-account-data-api-openapi.yml, openapi/xero-accounting-api-openapi.yml, openapi/xero-app-store-api-openapi.yml, openapi/xero-asset-api-openapi.yml, openapi/xero-bank-feeds-api-openapi.yml,\n  openapi/xero-bank-feeds-v2-api-openapi.yml, openapi/xero-files-api-openapi.yml, openapi/xero-finance-api-openapi.yml, openapi/xero-identity-api-openapi.yml, openapi/xero-payrollau-api-openapi.yml, openapi/xero-payrollau-v2-api-openapi.yml,\n  openapi/xero-payrollnz-api-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n    scopes: 3\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n  sources:\n  - openapi/xero-account-data-api-openapi.yml\n\
  \  - openapi/xero-accounting-api-openapi.yml\n  - openapi/xero-asset-api-openapi.yml\n  - openapi/xero-bank-feeds-api-openapi.yml\n  - openapi/xero-bank-feeds-v2-api-openapi.yml\n  - openapi/xero-files-api-openapi.yml\n  - openapi/xero-finance-api-openapi.yml\n  - openapi/xero-identity-api-openapi.yml\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollau-v2-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  - openapi/xero-project-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.xero.com/connect/token\n    scopes: 1\n  description: For more information\n  sources:\n  - openapi/xero-app-store-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/xero-identity-api-openapi.yml\ndocs: https://developer.xero.com/documentation/guides/oauth2/overview/\ndocumented_flows:\n- flow: authorization code (web apps)\n  docs:\
  \ https://developer.xero.com/documentation/guides/oauth2/auth-flow/\n- flow: PKCE (mobile/desktop/CLI)\n  docs: https://developer.xero.com/documentation/guides/oauth2/pkce-flow/\n- flow: client credentials (Custom Connections)\n  docs: https://developer.xero.com/documentation/guides/oauth2/custom-connections/\ntenant_header: xero-tenant-id (from the Connections endpoint after authorisation)\nrefresh: offline_access scope required for a refresh token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/authentication/xero-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
---
