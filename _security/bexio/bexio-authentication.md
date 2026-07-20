---
api_key_in: []
api_specs:
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Contacts API
  slug: bexio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Sales Order Management API
  slug: bexio-sales-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Accounting API
  slug: bexio-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Items API
  slug: bexio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Projects & Time Tracking API
  slug: bexio-projects-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Files API
  slug: bexio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Purchase API
  slug: bexio-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Payroll API
  slug: bexio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Banking API
  slug: bexio-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: probed
name: Bexio Authentication
name_suffix: Authentication
oauth_flows: []
overview: bexio secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: bexio
provider_slug: bexio
scheme_count: 2
schemes:
- authorizationUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/auth
  flow: authorizationCode
  issuer: https://auth.bexio.com/realms/bexio
  name: oauth2_authorization_code
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - company_profile
  - contact_show
  - contact_edit
  - kb_offer_show
  - kb_offer_edit
  - kb_order_show
  - kb_order_edit
  - kb_invoice_show
  - kb_invoice_edit
  - article_show
  - article_edit
  - accounting
  - project_show
  - project_edit
  - task_show
  - task_edit
  - file
  - kb_bill_show
  - kb_bill_edit
  - kb_expense_show
  - kb_expense_edit
  - payroll_employee_show
  - payroll_employee_edit
  - payroll_absence_show
  - payroll_absence_edit
  - bank_account_show
  - bank_payment_show
  sources:
  - https://auth.bexio.com/realms/bexio/.well-known/openid-configuration
  - https://developer.bexio.com/
  tokenUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/token
  type: oauth2
- bearerFormat: PAT
  name: personal_access_token
  scheme: bearer
  sources:
  - https://docs.bexio.com/
  - https://developer.bexio.com/
  type: http
slug: bexio-authentication
source_filename: bexio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: >-\n  https://auth.bexio.com/realms/bexio/.well-known/openid-configuration (live probe)\n  and https://docs.bexio.com/ / https://developer.bexio.com/\nsummary:\n  types:\n  - oauth2\n  - http\nnotes: >-\n  bexio supports two auth styles, both presented as an Authorization: Bearer\n  token against https://api.bexio.com/2.0. (1) OAuth 2.0 Authorization Code /\n  OpenID Connect via the Keycloak realm at https://auth.bexio.com/realms/bexio\n  for user-delegated app access. (2) Personal Access Tokens (PAT) for\n  server-to-server access. Fine-grained OAuth scopes gate each module\n  (contact_show/edit, kb_invoice_show/edit, accounting, project_show/edit,\n  payroll_employee_show/edit, etc.). offline_access grants refresh tokens.\nschemes:\n- name: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://auth.bexio.com/realms/bexio\n  authorizationUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/auth\n\
  \  tokenUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/token\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - company_profile\n  - contact_show\n  - contact_edit\n  - kb_offer_show\n  - kb_offer_edit\n  - kb_order_show\n  - kb_order_edit\n  - kb_invoice_show\n  - kb_invoice_edit\n  - article_show\n  - article_edit\n  - accounting\n  - project_show\n  - project_edit\n  - task_show\n  - task_edit\n  - file\n  - kb_bill_show\n  - kb_bill_edit\n  - kb_expense_show\n  - kb_expense_edit\n  - payroll_employee_show\n  - payroll_employee_edit\n  - payroll_absence_show\n  - payroll_absence_edit\n  - bank_account_show\n  - bank_payment_show\n  sources:\n  - https://auth.bexio.com/realms/bexio/.well-known/openid-configuration\n  - https://developer.bexio.com/\n- name: personal_access_token\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  sources:\n  - https://docs.bexio.com/\n  - https://developer.bexio.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/authentication/bexio-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Accounting
- ERP
- Invoicing
- SMB
- Switzerland
---
