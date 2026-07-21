---
api_key_in: []
api_specs:
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Product Reference Data API
  slug: bank-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Accounts & Balances API
  slug: bank-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Transactions API
  slug: bank-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: bank-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Payees API
  slug: bank-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bank Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bank Australia secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bank Australia
provider_slug: bank-australia
scheme_count: 2
schemes:
- applies_to: Product Reference Data API (GET /banking/products, /banking/products/{productId})
  description: Unauthenticated public endpoints. No credential is issued or required; the only mandatory request header is `x-v` (CDS API version).
  name: public-no-auth
  sources:
  - apis.yml
  type: none
- applies_to: Consumer Data Sharing (accredited data recipients, consenting customers)
  description: OAuth2 authorization-code + OIDC with mutual-TLS-bound tokens under the CDR security profile. Accreditation and dynamic client registration are handled via the CDR Register; not exercised by the public PRD API captured here.
  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  fapi_profile: FAPI 1.0 Advanced
  mtls: true
  name: cdr-oauth2-fapi
  pkce: true
  scheme: authorizationCode
  sources:
  - Consumer Data Standards security profile
  type: oauth2
slug: bank-australia-authentication
source_filename: bank-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://www.bankaust.com.au/support/open-banking/developer/ +\n  Consumer Data Standards (Consumer Data Right) security profile\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two distinct surfaces. The public Product Reference Data (PRD) API requires\n    NO authentication and NO API key - only the mandatory CDS `x-v` version\n    header. The authenticated Consumer Data Sharing surface (account and\n    transaction data for consenting customers) is governed by the CDR security\n    profile: OAuth2 authorization-code flow with OpenID Connect, mutual-TLS\n    sender-constrained tokens, PKCE, and the Financial-grade API (FAPI 1.0\n    Advanced) profile, brokered through the ACCC CDR Register rather than a\n    bank-proprietary authorization server.\nschemes:\n- name: public-no-auth\n  type: none\n  applies_to: Product Reference Data API (GET /banking/products,\
  \ /banking/products/{productId})\n  description: >-\n    Unauthenticated public endpoints. No credential is issued or required; the\n    only mandatory request header is `x-v` (CDS API version).\n  sources: [apis.yml]\n- name: cdr-oauth2-fapi\n  type: oauth2\n  scheme: authorizationCode\n  fapi_profile: FAPI 1.0 Advanced\n  mtls: true\n  pkce: true\n  applies_to: Consumer Data Sharing (accredited data recipients, consenting customers)\n  description: >-\n    OAuth2 authorization-code + OIDC with mutual-TLS-bound tokens under the CDR\n    security profile. Accreditation and dynamic client registration are handled\n    via the CDR Register; not exercised by the public PRD API captured here.\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  sources: [Consumer Data Standards security profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/authentication/bank-australia-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
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
