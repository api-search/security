---
api_key_in: []
api_specs:
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Product Reference Data API
  slug: rabobank-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Accounts & Balances API
  slug: rabobank-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Transactions API
  slug: rabobank-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Direct Debits & Scheduled Payments API
  slug: rabobank-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Payees API
  slug: rabobank-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
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
