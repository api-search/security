---
api_key_in: []
api_specs:
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Product Reference Data API
  slug: summerland-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Accounts & Balances API
  slug: summerland-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Transactions API
  slug: summerland-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Direct Debits & Scheduled Payments API
  slug: summerland-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Payees API
  slug: summerland-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Summerland Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Summerland Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Summerland Bank
provider_slug: summerland-bank
scheme_count: 0
schemes: []
slug: summerland-bank-authentication
source_filename: summerland-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.summerland.com.au/services/digital-and-payments/open-banking/\nnotes: >-\n  The harvested OpenAPI is the shared DSB Consumer Data Standards Banking API\n  contract, which declares no securitySchemes of its own; authentication for the\n  Consumer Data Right is defined by the separate CDR information security (InfoSec)\n  profile, not the resource-endpoint spec. Summerland Bank operates two distinct\n  auth postures, captured below.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nsurfaces:\n  - name: Public Product Reference Data (PRD)\n    base_url: https://public.cdr-api.summerland.com.au/cds-au/v1\n    auth: none\n    description: >-\n      GET /banking/products and GET /banking/products/{productId} are public and\n      unauthenticated per the CDR PRD requirement. No API key, token, or client\n      registration is required; only the mandatory\
  \ CDS `x-v` version header must\n      be supplied. Confirmed live 2026-07-20 (HTTP 200, x-v 5, 25 products).\n    operations: [listBankingProducts, getBankingProductDetail]\n  - name: Consumer data sharing (accredited data recipients)\n    base_url: https://mtls.dh.example.com/cds-au/v1\n    auth: oauth2 + openIdConnect + mutualTLS\n    profile: CDR InfoSec profile (FAPI 1.0 Advanced, OIDC Hybrid/PKCE, MTLS-bound tokens, JARM/PAR)\n    description: >-\n      Account, balance, transaction, direct-debit, scheduled-payment and payee\n      endpoints require an OAuth2 / OpenID Connect access token obtained by an\n      ACCC-accredited data recipient (ADR) under CDR consent, bound to the client\n      via mutual TLS. Not exposed as an open developer API; accessed by eligible\n      customers through the Summerland Bank app / internet banking. Governed by\n      the ACCC/OAIC and the DSB Consumer Data Standards security profile.\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n\
  schemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/authentication/summerland-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
---
