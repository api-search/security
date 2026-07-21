---
api_key_in: []
api_specs:
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Product Reference Data API
  slug: bank-of-queensland-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Accounts & Balances API
  slug: bank-of-queensland-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Transactions API
  slug: bank-of-queensland-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Direct Debits & Scheduled Payments API
  slug: bank-of-queensland-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Payees API
  slug: bank-of-queensland-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bank Of Queensland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank of Queensland secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bank of Queensland
provider_slug: bank-of-queensland
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: The Product Reference Data (PRD) endpoints are unauthenticated by CDR mandate - no API key, token, or client registration is required. Only the mandatory x-v version header must be supplied. Confirmed live at https://secure.api.boq.com.au/cds-au/v1/banking/products (HTTP 200).
  name: PublicProductReferenceData
  type: none
- applies_to:
  - listBankingAccounts
  - getBankingAccountDetail
  - getBankingBalance
  - listBankingTransactions
  - getBankingTransactionDetail
  - listBankingPayees
  - listScheduledPayments
  - listDirectDebits
  consumer_authentication: OTP-based consumer authorization (CDR authentication flows)
  description: 'All consumer data sharing (accounts, balances, transactions, payees, scheduled payments, direct debits) is gated behind the regulated CDR Accredited Data Recipient model: OAuth2 authorization-code with OpenID Connect, FAPI-grade security and MTLS-bound tokens. Access is restricted to ACCC-accredited data recipients - not open to arbitrary developers.'
  fapi_profile: FAPI 1.0 Advanced (Australia CDR security profile)
  name: CDRAccreditedDataRecipient
  scheme: authorizationCode
  token_binding: mutualTLS (MTLS-bound access tokens)
  type: oauth2
slug: bank-of-queensland-authentication
source_filename: bank-of-queensland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://www.boq.com.au/personal/help-and-support/forms-and-important-information/open-banking\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n# The harvested DSB CDS contract declares no securitySchemes (derive-authentication.py\n# returned an empty profile), so this profile is hand-authored from BOQ's public\n# CDR posture. It captures the two-tier CDR authorization model.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_prd_auth: none\n  consumer_data_auth: oauth2-oidc-fapi\nschemes:\n  - name: PublicProductReferenceData\n    type: none\n    applies_to: [listBankingProducts, getBankingProductDetail]\n    description: >-\n      The Product Reference Data (PRD) endpoints are unauthenticated by CDR\n      mandate - no API key, token, or client registration is required. Only the\n      mandatory x-v version header must be supplied. Confirmed live at\n      https://secure.api.boq.com.au/cds-au/v1/banking/products\
  \ (HTTP 200).\n  - name: CDRAccreditedDataRecipient\n    type: oauth2\n    scheme: authorizationCode\n    fapi_profile: FAPI 1.0 Advanced (Australia CDR security profile)\n    token_binding: mutualTLS (MTLS-bound access tokens)\n    consumer_authentication: OTP-based consumer authorization (CDR authentication flows)\n    applies_to:\n      - listBankingAccounts\n      - getBankingAccountDetail\n      - getBankingBalance\n      - listBankingTransactions\n      - getBankingTransactionDetail\n      - listBankingPayees\n      - listScheduledPayments\n      - listDirectDebits\n    description: >-\n      All consumer data sharing (accounts, balances, transactions, payees,\n      scheduled payments, direct debits) is gated behind the regulated CDR\n      Accredited Data Recipient model: OAuth2 authorization-code with OpenID\n      Connect, FAPI-grade security and MTLS-bound tokens. Access is restricted\n      to ACCC-accredited data recipients - not open to arbitrary developers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/authentication/bank-of-queensland-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
