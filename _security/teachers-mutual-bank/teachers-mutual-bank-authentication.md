---
api_key_in: []
api_specs:
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Product Reference Data API
  slug: teachers-mutual-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Accounts & Balances API
  slug: teachers-mutual-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Transactions API
  slug: teachers-mutual-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Direct Debits & Scheduled Payments API
  slug: teachers-mutual-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Payees API
  slug: teachers-mutual-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Teachers Mutual Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Teachers Mutual Bank secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Teachers Mutual Bank
provider_slug: teachers-mutual-bank
scheme_count: 2
schemes:
- applies_to:
  - openapi/teachers-mutual-bank-cds-banking-products-openapi.yml#listBankingProducts
  - openapi/teachers-mutual-bank-cds-banking-products-openapi.yml#getBankingProductDetail
  name: public-prd
  note: No authentication, no accreditation, no API key. Confirmed live HTTP 200.
  type: none
- flow: authorizationCode
  identity: openIdConnect
  name: cdr-consumer-channel
  note: Accredited Data Recipient (ADR) access only. Client registration and trust are established via the CDR Register; tokens carry CDR banking scopes (openid, bank:accounts.basic:read, bank:transactions:read, etc.). Not self-serve; no public credentials or sandbox are offered by the bank.
  scheme: FAPI 1.0
  type: oauth2
slug: teachers-mutual-bank-authentication
source_filename: teachers-mutual-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.tmbank.com.au/open-banking + review.yml + Consumer Data Standards CDR security profile\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two distinct channels. The public Product Reference Data (PRD) surface requires NO\n    authentication. The consumer data-sharing channel (accounts, balances, transactions,\n    direct debits, payees) is available only to CDR-accredited data recipients and uses\n    the OAuth2 / OpenID Connect FAPI 1.0 security profile mediated by the CDR Register.\nschemes:\n- name: public-prd\n  type: none\n  applies_to:\n  - openapi/teachers-mutual-bank-cds-banking-products-openapi.yml#listBankingProducts\n  - openapi/teachers-mutual-bank-cds-banking-products-openapi.yml#getBankingProductDetail\n  note: No authentication, no accreditation, no API key. Confirmed live HTTP 200.\n- name: cdr-consumer-channel\n  type: oauth2\n\
  \  scheme: FAPI 1.0\n  flow: authorizationCode\n  identity: openIdConnect\n  note: >-\n    Accredited Data Recipient (ADR) access only. Client registration and trust are\n    established via the CDR Register; tokens carry CDR banking scopes\n    (openid, bank:accounts.basic:read, bank:transactions:read, etc.). Not self-serve;\n    no public credentials or sandbox are offered by the bank.\ndocs: https://www.tmbank.com.au/open-banking\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/authentication/teachers-mutual-bank-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
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
