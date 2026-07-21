---
api_key_in: []
api_specs:
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Product Reference Data API
  slug: bank-of-melbourne-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Accounts & Balances API
  slug: bank-of-melbourne-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Transactions API
  slug: bank-of-melbourne-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Direct Debits & Scheduled Payments API
  slug: bank-of-melbourne-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Payees API
  slug: bank-of-melbourne-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Bank Of Melbourne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank of Melbourne declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Bank of Melbourne
provider_slug: bank-of-melbourne
scheme_count: 0
schemes: []
slug: bank-of-melbourne-authentication
source_filename: bank-of-melbourne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/bank-of-melbourne-cds-banking-products-openapi.yml\ndocs: https://www.bankofmelbourne.com.au/online-services/open-banking\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The harvested Bank of Melbourne CDR Banking OpenAPI declares NO\n    securitySchemes and applies NO security requirement to the public Product\n    Reference Data operations. The public PRD surface (listBankingProducts /\n    getBankingProductDetail) is unauthenticated by design under the Australian\n    Consumer Data Standards; the only required header is the mandatory x-v\n    version header.\nschemes: []\npublic_access:\n  authenticated: false\n  detail: >-\n    listBankingProducts and getBankingProductDetail are open, unauthenticated\n    GET endpoints served on shared Westpac Group infrastructure at\n    digital-api.bankofmelbourne.com.au.\nconsumer_data_sharing:\n  detail: >-\n    Access to consumer/account data beyond\
  \ product reference data (accounts,\n    balances, transactions, direct debits, scheduled payments, payees) is NOT\n    available through this public API. Although those operations appear in the\n    shared DSB spec, they are gated behind the CDR Accredited Data Recipient\n    (ADR) model, which uses an OAuth 2.0 / OpenID Connect, FAPI-hardened consent\n    flow operated through the CDR ecosystem (accreditation + the CDR Register)\n    rather than a Bank of Melbourne-issued developer credential. That surface is\n    out of scope for this public PRD contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/authentication/bank-of-melbourne-authentication.yml
summary_line: 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
- Westpac Group
---
