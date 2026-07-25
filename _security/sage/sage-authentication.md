---
api_key_in: []
api_specs:
- filename: sage-bank-accounts-api-openapi.yml
  format: yaml
  label: Sage Bank Accounts API
  slug: sage-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-bank-accounts-api-openapi.yml
- filename: sage-business-api-openapi.yml
  format: yaml
  label: Sage Business API
  slug: sage-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-business-api-openapi.yml
- filename: sage-contacts-api-openapi.yml
  format: yaml
  label: Sage Contacts API
  slug: sage-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-contacts-api-openapi.yml
- filename: sage-ledger-accounts-api-openapi.yml
  format: yaml
  label: Sage Ledger Accounts API
  slug: sage-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-ledger-accounts-api-openapi.yml
- filename: sage-payments-api-openapi.yml
  format: yaml
  label: Sage Payments API
  slug: sage-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-payments-api-openapi.yml
- filename: sage-products-api-openapi.yml
  format: yaml
  label: Sage Products API
  slug: sage-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-products-api-openapi.yml
- filename: sage-purchase-invoices-api-openapi.yml
  format: yaml
  label: Sage Purchase Invoices API
  slug: sage-purchase-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-purchase-invoices-api-openapi.yml
- filename: sage-sales-invoices-api-openapi.yml
  format: yaml
  label: Sage Sales Invoices API
  slug: sage-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-sales-invoices-api-openapi.yml
- filename: sage-tax-rates-api-openapi.yml
  format: yaml
  label: Sage Tax Rates API
  slug: sage-tax-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-tax-rates-api-openapi.yml
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
