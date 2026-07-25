---
api_key_in: []
api_specs:
- filename: greater-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Balances API
  slug: greater-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-balances-api-openapi.yml
- filename: greater-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Direct Debits API
  slug: greater-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-direct-debits-api-openapi.yml
- filename: greater-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Scheduled Payments API
  slug: greater-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: greater-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Transactions API
  slug: greater-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-transactions-api-openapi.yml
- filename: greater-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Accounts API
  slug: greater-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-accounts-api-openapi.yml
- filename: greater-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Payees API
  slug: greater-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-payees-api-openapi.yml
- filename: greater-bank-banking-products-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Products API
  slug: greater-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Greater Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Greater Bank secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Greater Bank
provider_slug: greater-bank
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  detail: Public, unauthenticated, read-only. Only the mandatory x-v version header is required; no credentials, no OAuth, no API key.
  name: PublicPRD
  sources:
  - openapi/greater-bank-cds-banking-products-openapi.yml
  type: none
- applies_to:
  - authenticated CDR consumer-data sharing (accounts/balances/transactions/payees)
  detail: Accredited data recipients obtain consumer consent and access tokens through the CDR register and Greater Bank's info-security endpoints (authorization/token). Documented via the CDR regime, not exposed as a self-serve public developer OAuth surface. Not independently probed.
  name: CDR-ADR-OAuth2-OIDC-FAPI
  scheme_profile: FAPI 2.0 / OpenID Connect
  sources:
  - review.yml
  type: oauth2
slug: greater-bank-authentication
source_filename: greater-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/greater-bank-cds-banking-products-openapi.yml\nnote: >-\n  The harvested spec declares no securitySchemes because Greater Bank's public\n  CDR Product Reference Data endpoints are unauthenticated by design. The\n  broader CDR consumer-data-sharing tier (not part of this public spec) is\n  secured under the accredited-data-recipient model with OAuth2 + OpenID Connect\n  on the FAPI profile via the CDR register.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  public_prd: unauthenticated\n  oauth2_flows: [authorizationCode]     # authenticated CDR data-sharing tier only\nschemes:\n  - name: PublicPRD\n    type: none\n    applies_to: [listBankingProducts, getBankingProductDetail]\n    detail: >-\n      Public, unauthenticated, read-only. Only the mandatory x-v version header\n      is required; no credentials, no OAuth, no API key.\n    sources: [openapi/greater-bank-cds-banking-products-openapi.yml]\n  - name: CDR-ADR-OAuth2-OIDC-FAPI\n\
  \    type: oauth2\n    scheme_profile: FAPI 2.0 / OpenID Connect\n    applies_to: [authenticated CDR consumer-data sharing (accounts/balances/transactions/payees)]\n    detail: >-\n      Accredited data recipients obtain consumer consent and access tokens\n      through the CDR register and Greater Bank's info-security endpoints\n      (authorization/token). Documented via the CDR regime, not exposed as a\n      self-serve public developer OAuth surface. Not independently probed.\n    sources: [review.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/authentication/greater-bank-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Product Reference Data
---
