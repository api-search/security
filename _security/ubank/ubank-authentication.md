---
api_key_in: []
api_specs:
- filename: ubank-banking-account-balances-api-openapi.yml
  format: yaml
  label: ubank Banking Account Balances API
  slug: ubank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-account-balances-api-openapi.yml
- filename: ubank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: ubank Banking Account Direct Debits API
  slug: ubank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-account-direct-debits-api-openapi.yml
- filename: ubank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: ubank Banking Account Scheduled Payments API
  slug: ubank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-account-scheduled-payments-api-openapi.yml
- filename: ubank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: ubank Banking Account Transactions API
  slug: ubank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-account-transactions-api-openapi.yml
- filename: ubank-banking-accounts-api-openapi.yml
  format: yaml
  label: ubank Banking Accounts API
  slug: ubank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-accounts-api-openapi.yml
- filename: ubank-banking-payees-api-openapi.yml
  format: yaml
  label: ubank Banking Payees API
  slug: ubank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-payees-api-openapi.yml
- filename: ubank-banking-products-api-openapi.yml
  format: yaml
  label: ubank Banking Products API
  slug: ubank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ubank Authentication
name_suffix: Authentication
oauth_flows: []
overview: ubank secures its APIs with none, oauth2, and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ubank
provider_slug: ubank
scheme_count: 0
schemes: []
slug: ubank-authentication
source_filename: ubank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  DSB Consumer Data Standards security profile and the ubank CDR pages. The\n  harvested OpenAPI declares no securitySchemes because the two operations ubank\n  exposes publicly are the unauthenticated Product Reference Data endpoints; the\n  authenticated CDR consumer-data surface is governed by the CDR FAPI security\n  profile and is not part of the public API.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [none, oauth2, openIdConnect]\n  public_surface: none\n  authenticated_surface: oauth2 + openIdConnect (FAPI)\nsurfaces:\n- name: public-product-reference-data\n  auth: none\n  applies_to: [listBankingProducts, getBankingProductDetail]\n  detail: >-\n    Public, unauthenticated CDR Product Reference Data. No API key, token, or\n    client credential is required. Requests must carry an x-v version header.\n- name: authenticated-cdr-data-sharing\n  auth: oauth2\
  \ + openid-connect\n  security_profile: FAPI (Financial-grade API)\n  applies_to: not-publicly-accessible\n  detail: >-\n    Consumer banking data (accounts, balances, transactions, payees, scheduled\n    payments, direct debits) is shared only with CDR Accredited Data Recipients\n    (ADRs) after consumer consent, via the CDR OAuth2/OpenID Connect FAPI\n    authorization model. Not exposed on ubank's public API surface and not\n    exercisable without CDR accreditation.\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/authentication/ubank-authentication.yml
summary_line: none/oauth2/openIdConnect · 0 schemes
tags:
- Financial
- Banks
- Banking
- Open Banking
- CDR
- Consumer Data Right
- Product Reference Data
- Digital Bank
- Consumer Banking
- Australia
---
