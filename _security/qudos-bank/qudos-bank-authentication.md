---
api_key_in: []
api_specs:
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Product Reference Data API
  slug: qudos-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Accounts & Balances API
  slug: qudos-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Transactions API
  slug: qudos-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Direct Debits & Scheduled Payments API
  slug: qudos-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Payees API
  slug: qudos-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Qudos Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qudos Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qudos Bank
provider_slug: qudos-bank
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  name: none-public-prd
  type: none
- applies_to: cdr-consumer-data-sharing
  flow: authorizationCode
  name: cdr-fapi
  profile: FAPI 2.0
  transport: mutualTLS
  type: oauth2
slug: qudos-bank-authentication
source_filename: qudos-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://www.qudosbank.com.au/support/open-banking +\n  https://consumerdatastandardsaustralia.github.io/standards/\ndocs: https://www.qudosbank.com.au/support/open-banking\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_prd: unauthenticated\n  data_sharing: fapi-2.0\nsurfaces:\n- name: Product Reference Data (PRD)\n  operations: [listBankingProducts, getBankingProductDetail]\n  auth: none\n  description: >-\n    Public, unauthenticated. No API key, token, or client certificate required.\n    Requests must send the x-v version header. Confirmed live returning HTTP 200\n    at https://public.cdr.qudosbank.com.au/cds-au/v1/banking/products.\n- name: CDR consumer data sharing\n  operations: [listBankingAccounts, getBankingAccountDetail, listBankingTransactions, getBankingBalance, listDirectDebits, listScheduledPayments, listBankingPayees]\n  auth: oauth2 + openIdConnect over mutualTLS (FAPI 2.0)\n \
  \ description: >-\n    The account/transaction/payments/payees operations require CDR consumer data\n    sharing authorization: an accredited data recipient (ACCC-accredited) obtains\n    the customer's consent via OAuth 2.0 authorization code flow with OpenID\n    Connect, PKCE/PAR, and mutual TLS client authentication under the Data\n    Standards Body FAPI security profile. Discovery and trust is brokered by the\n    ACCC CDR Register, not a per-holder /.well-known/openid-configuration.\n  register: https://consumerdatastandardsaustralia.github.io/register/\nschemes:\n- name: none-public-prd\n  type: none\n  applies_to: [listBankingProducts, getBankingProductDetail]\n- name: cdr-fapi\n  type: oauth2\n  flow: authorizationCode\n  profile: FAPI 2.0\n  transport: mutualTLS\n  applies_to: cdr-consumer-data-sharing\nnotes: >-\n  The harvested OpenAPI declares no components.securitySchemes because the\n  public PRD subset is unauthenticated by CDR mandate; the FAPI-secured data\n  sharing\
  \ surface is governed by the CDR Register and Data Standards rather than\n  inline OpenAPI security schemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/authentication/qudos-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Mutual Bank
- Product Reference Data
---
