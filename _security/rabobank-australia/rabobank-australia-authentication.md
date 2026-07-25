---
api_key_in: []
api_specs:
- filename: rabobank-australia-banking-account-balances-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Balances API
  slug: rabobank-australia-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-balances-api-openapi.yml
- filename: rabobank-australia-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Direct Debits API
  slug: rabobank-australia-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-direct-debits-api-openapi.yml
- filename: rabobank-australia-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Scheduled Payments API
  slug: rabobank-australia-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-scheduled-payments-api-openapi.yml
- filename: rabobank-australia-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Transactions API
  slug: rabobank-australia-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-transactions-api-openapi.yml
- filename: rabobank-australia-banking-accounts-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Accounts API
  slug: rabobank-australia-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-accounts-api-openapi.yml
- filename: rabobank-australia-banking-payees-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Payees API
  slug: rabobank-australia-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-payees-api-openapi.yml
- filename: rabobank-australia-banking-products-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Products API
  slug: rabobank-australia-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Rabobank Australia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rabobank Australia secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rabobank Australia
provider_slug: rabobank-australia
scheme_count: 2
schemes:
- applies_to:
  - openapi/rabobank-australia-cds-banking-products-openapi.yml#listBankingProducts
  - openapi/rabobank-australia-cds-banking-products-openapi.yml#getBankingProductDetail
  detail: 'Product Reference Data endpoints are public and unauthenticated by CDR design. Confirmed live: GET /banking/products succeeds with only the mandatory x-v header and no credentials.'
  name: public-prd
  type: none
- applies_to: authenticated CDR consumer data sharing (accounts, balances, transactions, payees, direct debits)
  detail: Not a self-serve public API. Authenticated CDR data sharing is available only to accredited data recipients (ADRs) under the Consumer Data Right, with Rabobank Australia acting as a registered data holder. Consent is obtained through the CDR OAuth2 / OpenID Connect (FAPI) authorization flow; access tokens are scoped to CDR banking scopes (bank:accounts.basic:read, bank:transactions:read, common:customer.basic:read, etc.).
  name: cdr-adr-oauth2-oidc-fapi
  scheme_detail: OpenID Connect Hybrid flow with FAPI 1.0 Advanced security profile, PAR, PKCE and mTLS-bound tokens.
  type: oauth2
slug: rabobank-australia-authentication
source_filename: rabobank-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  Rabobank Australia Open Banking pages + CDR regime + live probe (no auth\n  required on GET /banking/products). The harvested CDS OpenAPI declares no\n  securitySchemes for the public PRD paths.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  public_surface_auth: none\n  authenticated_surface_auth: [oauth2, openIdConnect]\nschemes:\n- name: public-prd\n  type: none\n  applies_to:\n  - openapi/rabobank-australia-cds-banking-products-openapi.yml#listBankingProducts\n  - openapi/rabobank-australia-cds-banking-products-openapi.yml#getBankingProductDetail\n  detail: >-\n    Product Reference Data endpoints are public and unauthenticated by CDR\n    design. Confirmed live: GET /banking/products succeeds with only the\n    mandatory x-v header and no credentials.\n- name: cdr-adr-oauth2-oidc-fapi\n  type: oauth2\n  scheme_detail: OpenID Connect Hybrid flow with FAPI 1.0 Advanced security profile, PAR, PKCE and mTLS-bound\
  \ tokens.\n  applies_to: authenticated CDR consumer data sharing (accounts, balances, transactions, payees, direct debits)\n  detail: >-\n    Not a self-serve public API. Authenticated CDR data sharing is available\n    only to accredited data recipients (ADRs) under the Consumer Data Right,\n    with Rabobank Australia acting as a registered data holder. Consent is\n    obtained through the CDR OAuth2 / OpenID Connect (FAPI) authorization flow;\n    access tokens are scoped to CDR banking scopes (bank:accounts.basic:read,\n    bank:transactions:read, common:customer.basic:read, etc.).\ndocs: https://www.rabobank.com.au/support/open-banking\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/authentication/rabobank-australia-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Agribusiness
- Product Reference Data
---
