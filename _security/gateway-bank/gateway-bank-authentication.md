---
api_key_in: []
api_specs:
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Product Reference Data API
  slug: gateway-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Accounts & Balances API
  slug: gateway-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Transactions API
  slug: gateway-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Direct Debits & Scheduled Payments API
  slug: gateway-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Payees API
  slug: gateway-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Gateway Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gateway Bank secures its APIs with none, oauth2, and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gateway Bank
provider_slug: gateway-bank
scheme_count: 0
schemes: []
slug: gateway-bank-authentication
source_filename: gateway-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: DSB Consumer Data Standards CDR security profile + openapi x-scopes + review.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: Two distinct surfaces. The public Product Reference Data (PRD) endpoints are\n    deliberately UNAUTHENTICATED per the Consumer Data Standards (product data carries\n    no consumer information). All consumer-data endpoints (accounts, balances,\n    transactions, direct debits, scheduled payments, payees, instalment plans) are\n    gated by the CDR security profile, an OpenID Connect / FAPI 2.0 flow restricted\n    to ACCC-accredited Data Recipients operating against the CDR Register.\nsurfaces:\n- name: public-prd\n  authentication: none\n  description: GET /banking/products and GET /banking/products/{productId} require no\n    credentials. Only the\
  \ CDS version header (x-v) is mandatory.\n  operations: [listBankingProducts, getBankingProductDetail]\n- name: cdr-consumer-data\n  authentication: oauth2 + openIdConnect (FAPI)\n  profile: CDR security profile (FAPI 2.0 baseline)\n  flows:\n  - flow: authorizationCode\n    grant: authorization_code\n    features: [PAR, PKCE, private_key_jwt or MTLS client auth]\n    authorizationUrl: via the bank's CDR InfoSec endpoints published to the CDR Register\n    tokenUrl: via the bank's CDR InfoSec endpoints published to the CDR Register\n  eligibility: ACCC-accredited Data Recipients (ADR) only; not a self-serve developer\n    surface.\n  scopes_ref: scopes/gateway-bank-scopes.yml\n  operations:\n  - listBankingAccounts\n  - getBankingAccountDetail\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n  - getBankingBalance\n  - listBankingTransactions\n  - getBankingTransactionDetail\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  -\
  \ listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n  - listBankingPayees\n  - getBankingPayeeDetail\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/authentication/gateway-bank-authentication.yml
summary_line: none/oauth2/openIdConnect · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Customer Owned
- Australia
- Product Reference Data
---
