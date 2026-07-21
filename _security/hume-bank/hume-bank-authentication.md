---
api_key_in: []
api_specs:
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Product Reference Data API
  slug: hume-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Accounts & Balances API
  slug: hume-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Transactions API
  slug: hume-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Direct Debits & Scheduled Payments API
  slug: hume-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Payees API
  slug: hume-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Hume Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hume Bank secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hume Bank
provider_slug: hume-bank
scheme_count: 0
schemes: []
slug: hume-bank-authentication
source_filename: hume-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.humebank.com.au/about-hume-bank/customer-resources/open-banking-products-api\ndocs: https://www.humebank.com.au/about-hume-bank/customer-resources/open-banking-products-api\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The Product Reference Data (PRD) endpoints of the Australian Consumer Data\n    Right are public and unauthenticated by design. No API key, OAuth token, or\n    client registration is required to call GET /banking/products or\n    GET /banking/products/{productId}. Callers MUST send the mandatory x-v\n    request header (API version) per the Consumer Data Standards.\nschemes: []\nnotes:\n  - The broader CDR consumer-data flows (accounts, transactions) that Hume Bank\n    operates as a data holder DO require OAuth2 / OIDC (FAPI) and accreditation\n    with the ACCC as an Accredited Data Recipient; those flows are not part of\n    this public PRD spec and are gated\
  \ through the CDR Register.\n  - Public PRD access is rate-managed and unauthenticated; see conventions/ for\n    the required version-negotiation headers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/authentication/hume-bank-authentication.yml
summary_line: none · 0 schemes
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
