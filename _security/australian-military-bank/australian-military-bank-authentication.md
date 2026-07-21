---
api_key_in: []
api_specs:
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Product Reference Data API
  slug: australian-military-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Accounts & Balances API
  slug: australian-military-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Transactions API
  slug: australian-military-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Direct Debits & Scheduled Payments API
  slug: australian-military-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Payees API
  slug: australian-military-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Australian Military Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Military Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australian Military Bank
provider_slug: australian-military-bank
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: 'Public, unauthenticated Product Reference Data. No API key, token, or client certificate is required. Callers MUST send an x-v header to negotiate the endpoint version (currently x-v: 3 for products).'
  name: public-prd
  type: none
- description: 'Consumer data sharing uses the CDR security profile: OpenID Connect hybrid/authorization-code flow with PAR, mTLS-bound access tokens, and the AU adaptations of FAPI. Access is limited to software products registered with the CDR Register and accredited by the ACCC/OAIC. Not exercisable via this public repo.'
  name: cdr-fapi
  profile: FAPI 2.0 (AU-CDR)
  scheme: authorization_code
  scopes:
  - bank:accounts.basic:read
  - bank:accounts.detail:read
  - bank:transactions:read
  - bank:regular_payments:read
  - bank:payees:read
  - common:customer.basic:read
  token_binding: mutualTLS
  type: oauth2
slug: australian-military-bank-authentication
source_filename: australian-military-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_surface: unauthenticated\n  authenticated_surface: cdr-fapi\nnotes: >-\n  The OpenAPI in this repo is the Data Standards Body CDR Banking API. Only the\n  Product Reference Data (PRD) endpoints (GET /banking/products and\n  GET /banking/products/{productId}) are exposed on Australian Military Bank's\n  public host and they require NO authentication. All consumer-data endpoints\n  (accounts, balances, transactions, direct debits, scheduled payments, payees)\n  are available only to CDR-accredited data recipients over the authenticated,\n  FAPI-profiled CDR data-holder flow; the spec documents the required CDR scopes\n  as x-scopes extensions (bank:accounts.basic:read, bank:accounts.detail:read,\n\
  \  bank:transactions:read, bank:regular_payments:read, bank:payees:read) but\n  declares no formal OpenAPI securitySchemes.\nschemes:\n  - name: public-prd\n    type: none\n    applies_to:\n      - listBankingProducts\n      - getBankingProductDetail\n    description: >-\n      Public, unauthenticated Product Reference Data. No API key, token, or\n      client certificate is required. Callers MUST send an x-v header to\n      negotiate the endpoint version (currently x-v: 3 for products).\n  - name: cdr-fapi\n    type: oauth2\n    scheme: authorization_code\n    profile: FAPI 2.0 (AU-CDR)\n    token_binding: mutualTLS\n    description: >-\n      Consumer data sharing uses the CDR security profile: OpenID Connect\n      hybrid/authorization-code flow with PAR, mTLS-bound access tokens, and\n      the AU adaptations of FAPI. Access is limited to software products\n      registered with the CDR Register and accredited by the ACCC/OAIC. Not\n      exercisable via this public repo.\n    scopes:\n\
  \      - bank:accounts.basic:read\n      - bank:accounts.detail:read\n      - bank:transactions:read\n      - bank:regular_payments:read\n      - bank:payees:read\n      - common:customer.basic:read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/authentication/australian-military-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Defence
---
