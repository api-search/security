---
api_key_in: []
api_specs:
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Deals API
  slug: freee-accounting-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Account Items API
  slug: freee-accounting-account-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Partners API
  slug: freee-accounting-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Invoices and Quotations API
  slug: freee-accounting-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Wallet Transactions API
  slug: freee-accounting-wallet-txns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Journals and Reports API
  slug: freee-accounting-journals-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Employees API
  slug: freee-hr-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Payroll API
  slug: freee-hr-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Attendance API
  slug: freee-hr-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Freee Authentication
name_suffix: Authentication
oauth_flows: []
overview: freee secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: freee
provider_slug: freee
scheme_count: 1
schemes:
- authorizationUrl: https://accounts.secure.freee.co.jp/public_api/authorize
  description: 'freee unified OAuth 2.0. Register an application in the freee Developers console to obtain a client_id and client_secret, send the user through the authorization code grant, then exchange the code for an access token and refresh token. The access token is presented on every API request as `Authorization: Bearer <access_token>`. A single freee token works across products (accounting, HR/payroll, invoicing) subject to the granted scopes. Access tokens are short-lived and are renewed with the refresh token.'
  grantType: authorization_code
  name: oauth2
  scopes:
  - description: データの読み取り (read data)
    name: read
  - description: データの書き込み (write data)
    name: write
  sources:
  - openapi/freee-openapi.yml
  - https://developer.freee.co.jp/reference/accounting/reference
  - https://github.com/freee/freee-api-schema
  tokenUrl: https://accounts.secure.freee.co.jp/public_api/token
  type: oauth2
slug: freee-authentication
source_filename: freee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/freee-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2\n  type: oauth2\n  grantType: authorization_code\n  description: >-\n    freee unified OAuth 2.0. Register an application in the freee Developers\n    console to obtain a client_id and client_secret, send the user through the\n    authorization code grant, then exchange the code for an access token and\n    refresh token. The access token is presented on every API request as\n    `Authorization: Bearer <access_token>`. A single freee token works across\n    products (accounting, HR/payroll, invoicing) subject to the granted scopes.\n    Access tokens are short-lived and are renewed with the refresh token.\n  authorizationUrl: https://accounts.secure.freee.co.jp/public_api/authorize\n  tokenUrl: https://accounts.secure.freee.co.jp/public_api/token\n  scopes:\n  - name: read\n    description: データの読み取り (read data)\n  - name: write\n    description:\
  \ データの書き込み (write data)\n  sources:\n  - openapi/freee-openapi.yml\n  - https://developer.freee.co.jp/reference/accounting/reference\n  - https://github.com/freee/freee-api-schema\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/authentication/freee-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Bookkeeping
- HR
- Payroll
- Invoicing
- Finance
- SaaS
- Japan
---
