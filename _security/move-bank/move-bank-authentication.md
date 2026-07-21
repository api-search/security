---
api_key_in: []
api_specs:
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Product Reference Data API
  slug: move-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Accounts & Balances API
  slug: move-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Transactions API
  slug: move-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Direct Debits & Scheduled Payments API
  slug: move-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Payees API
  slug: move-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Move Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: MOVE Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MOVE Bank
provider_slug: move-bank
scheme_count: 0
schemes: []
slug: move-bank-authentication
source_filename: move-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >\n  https://www.movebank.com.au/about-us/corporate-information/open-banking/ +\n  Consumer Data Standards (consumerdatastandardsaustralia.github.io/standards) +\n  CDR Security Profile; OpenAPI declares no securitySchemes (the Get Products\n  endpoint is public/unauthenticated by CDR mandate).\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  model: two-tier\n  public_prd: unauthenticated\n  consumer_sharing: cdr-security-profile\ntiers:\n- name: Product Reference Data (PRD)\n  authentication: none\n  description: >\n    The public Product Reference Data API (Get Products / Get Product Detail\n    under /cds-au/v1/banking/products) is unauthenticated by design — a CDR data\n    holder obligation. No API key, token, or client credential is required;\n    callers supply only the CDS version header x-v (currently 4 for Get Products).\n  operations: [listBankingProducts, getBankingProductDetail]\n  confirmed: true\n\
  - name: Consumer Data Sharing (accounts, balances, transactions, direct debits, scheduled payments, payees)\n  authentication: oauth2 + openIdConnect + mutualTLS\n  profile: CDR Security Profile (FAPI 1.0 Advanced-based, OIDC Hybrid flow, PAR, PKCE, private_key_jwt)\n  description: >\n    All non-PRD banking resources require the CDR Accredited Data Recipient (ADR)\n    model: the caller must be ACCC-accredited, hold consumer consent, and present\n    a token obtained under the CDR Security Profile over mutual TLS. This surface\n    is not publicly documented by MOVE Bank; it is governed centrally by the DSB\n    Consumer Data Standards and the CDR Register. Joint-account data sharing is\n    noted by the bank as not currently available.\n  operations: [listBankingAccounts, getBankingAccountDetail, getBankingBalance, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, listBankingTransactions, getBankingTransactionDetail, listDirectDebits, listScheduledPayments, listBankingPayees,\
  \ getBankingPayeeDetail]\nschemes: []\nnotes: >\n  The harvested OpenAPI is the shared DSB CDR Banking API standard (v1.36.0),\n  which intentionally omits securitySchemes (auth is defined by the separate CDR\n  Security Profile, not per-resource in the spec). derive-authentication.py\n  therefore found 0 schemes; this profile is the searched upgrade documenting the\n  real two-tier model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/authentication/move-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Australia
- Product Reference Data
---
