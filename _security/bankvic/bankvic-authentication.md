---
api_key_in: []
api_specs:
- filename: bankvic-banking-account-balances-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Balances API
  slug: bankvic-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-balances-api-openapi.yml
- filename: bankvic-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Direct Debits API
  slug: bankvic-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-direct-debits-api-openapi.yml
- filename: bankvic-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Scheduled Payments API
  slug: bankvic-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-scheduled-payments-api-openapi.yml
- filename: bankvic-banking-account-transactions-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Transactions API
  slug: bankvic-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-transactions-api-openapi.yml
- filename: bankvic-banking-accounts-api-openapi.yml
  format: yaml
  label: BankVic Banking Accounts API
  slug: bankvic-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-accounts-api-openapi.yml
- filename: bankvic-banking-payees-api-openapi.yml
  format: yaml
  label: BankVic Banking Payees API
  slug: bankvic-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-payees-api-openapi.yml
- filename: bankvic-banking-products-api-openapi.yml
  format: yaml
  label: BankVic Banking Products API
  slug: bankvic-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-products-api-openapi.yml
auth_types:
- none-public
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bankvic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BankVic secures its APIs with none-public, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BankVic
provider_slug: bankvic
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  detail: Public, unauthenticated. Only the mandatory `x-v` version-negotiation request header is required (optional `x-min-v`). No API key, no OAuth token, no mTLS.
  name: PRD (Product Reference Data)
  sources:
  - openapi/bankvic-cds-banking-products-openapi.yml
  type: none
- conforms:
  - FAPI 2.0
  - OIDC
  - PKCE
  - mTLS
  - RFC 9126 PAR
  detail: 'Consented account/transaction/balance/direct-debit/scheduled-payment/payee data is shared only via an accredited Data Recipient using the CDR security profile: OpenID Connect + OAuth 2.0 authorization code flow with PKCE, PAR, mTLS-bound sender-constrained access tokens, and CDR-issued client registration (DCR). BankVic acts as the Data Holder; there is no self-service developer OAuth client for the general public.'
  name: CDR Consumer Data Sharing (FAPI 2.0 profile)
  scheme: authorizationCode
  sources:
  - https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: oauth2
slug: bankvic-authentication
source_filename: bankvic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.bankvic.com.au/get-help/open-banking/\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  The OpenAPI contract in this repo (the shared DSB CDR Banking API) declares no\n  securitySchemes, because it documents both the public Product Reference Data (PRD)\n  surface and the consented consumer-data surface in one file. BankVic's exposed\n  public API — GET /banking/products and GET /banking/products/{productId} — is\n  UNAUTHENTICATED by CDR rule (PRD requires no consumer authorisation and no client\n  credentials; confirmed live returning HTTP 200 with only the mandatory x-v request\n  header). The authenticated consumer-data-sharing surface is not directly callable\n  by third parties: it is reached only through an accredited Data Recipient (ADR)\n  under the CDR security profile.\nsummary:\n  types: [none-public, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n\
  \  oauth2_flows: [authorizationCode]\n  public_endpoints_unauthenticated: true\nschemes:\n  - name: PRD (Product Reference Data)\n    type: none\n    applies_to: [listBankingProducts, getBankingProductDetail]\n    detail: >-\n      Public, unauthenticated. Only the mandatory `x-v` version-negotiation request\n      header is required (optional `x-min-v`). No API key, no OAuth token, no mTLS.\n    sources: [openapi/bankvic-cds-banking-products-openapi.yml]\n  - name: CDR Consumer Data Sharing (FAPI 2.0 profile)\n    type: oauth2\n    scheme: authorizationCode\n    detail: >-\n      Consented account/transaction/balance/direct-debit/scheduled-payment/payee data\n      is shared only via an accredited Data Recipient using the CDR security profile:\n      OpenID Connect + OAuth 2.0 authorization code flow with PKCE, PAR, mTLS-bound\n      sender-constrained access tokens, and CDR-issued client registration (DCR).\n      BankVic acts as the Data Holder; there is no self-service developer OAuth\
  \ client\n      for the general public.\n    conforms: [FAPI 2.0, OIDC, PKCE, mTLS, RFC 9126 PAR]\n    sources: [https://consumerdatastandardsaustralia.github.io/standards/#security-profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/authentication/bankvic-authentication.yml
summary_line: none-public/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
