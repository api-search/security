---
api_key_in: []
api_specs:
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Product Reference Data API
  slug: pn-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Accounts & Balances API
  slug: pn-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Transactions API
  slug: pn-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Direct Debits & Scheduled Payments API
  slug: pn-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Payees API
  slug: pn-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Common Discovery API
  slug: pn-bank-cdr-common-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Pn Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: P&N Bank secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: P&N Bank
provider_slug: pn-bank
scheme_count: 0
schemes: []
slug: pn-bank-authentication
source_filename: pn-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pn-bank-cds-banking-products-openapi.yml\ndocs: https://www.pnbank.com.au/help-and-support/open-banking/pn-bank-products-api/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    P&N Bank's public Product Reference Data (PRD) API is UNAUTHENTICATED: no API key,\n    token, or client credentials are required. The OpenAPI declares no\n    securitySchemes. This is by CDR design — product reference data is public.\nschemes: []\nauthenticated_data_sharing:\n  applies_to: >-\n    Consumer data sharing beyond product reference data (accounts, balances,\n    transactions, direct debits, scheduled payments, payees).\n  model: CDR OAuth2 / OpenID Connect (FAPI 1.0 Advanced) authorization\n  access: >-\n    Restricted to accredited data recipients (ADRs) via the CDR Register; the data\n    holder authorization server and its discovery documents are not part of the\n    public PRD surface probed here.\n\
  \  reference: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/authentication/pn-bank-authentication.yml
summary_line: none · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
---
