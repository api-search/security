---
api_key_in: []
api_specs:
- filename: bank-first-cds-banking-products-openapi.yml
  format: yaml
  label: Bank First CDR Product Reference Data API
  slug: bank-first-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-cds-banking-products-openapi.yml
- filename: bank-first-cds-banking-products-openapi.yml
  format: yaml
  label: Bank First CDR Accounts & Balances API
  slug: bank-first-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-cds-banking-products-openapi.yml
- filename: bank-first-cds-banking-products-openapi.yml
  format: yaml
  label: Bank First CDR Transactions API
  slug: bank-first-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-cds-banking-products-openapi.yml
- filename: bank-first-cds-banking-products-openapi.yml
  format: yaml
  label: Bank First CDR Direct Debits & Scheduled Payments API
  slug: bank-first-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-cds-banking-products-openapi.yml
- filename: bank-first-cds-banking-products-openapi.yml
  format: yaml
  label: Bank First CDR Payees API
  slug: bank-first-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bank First Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank First secures its APIs with none, oauth2, and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bank First
provider_slug: bank-first
scheme_count: 1
schemes:
- applies_to: Consumer Data Sharing
  dynamic_client_registration: CDR Register (ACCC)
  fapi: true
  flow: authorizationCode
  mtls: true
  name: CDR-OAuth2-OIDC-FAPI
  pkce: required
  type: oauth2
slug: bank-first-authentication
source_filename: bank-first-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.bankfirst.com.au/open-banking\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [none, oauth2, openIdConnect]\n  note: >-\n    Two distinct surfaces. The public Product Reference Data (PRD) API is fully\n    unauthenticated. The consumer data sharing surface (accounts/balances/\n    transactions) is gated behind CDR accreditation and uses OAuth 2.0 / OpenID\n    Connect hardened to the FAPI profile per the CDR security profile.\nsurfaces:\n  - name: Product Reference Data (PRD)\n    baseURL: https://public.cdr.bankfirst.com.au/cds-au/v1/banking\n    auth: none\n    detail: >-\n      Public, unauthenticated. No API key, client registration, or token\n      required. Clients send an x-v (API version) header; the response echoes the\n      served payload version in x-v. Confirmed live HTTP 200.\n  - name: Consumer Data Sharing\n    baseURL: https://developer.cdr.bankfirst.com.au/\n\
  \    auth: oauth2\n    detail: >-\n      Restricted to Accredited Data Recipients (ADRs). Access is via the CDR\n      consent flow: OAuth 2.0 authorization-code with PKCE and OpenID Connect,\n      hardened to FAPI (CDR security profile), with mutual-TLS sender-constrained\n      tokens and register-based dynamic client registration through the ACCC CDR\n      Register. Customers never share their banking credentials with third\n      parties. Host did not respond to unauthenticated probing (gated).\n    scopes_ref: scopes/bank-first-scopes.yml\nschemes:\n  - name: CDR-OAuth2-OIDC-FAPI\n    type: oauth2\n    flow: authorizationCode\n    pkce: required\n    fapi: true\n    mtls: true\n    dynamic_client_registration: CDR Register (ACCC)\n    applies_to: Consumer Data Sharing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/authentication/bank-first-authentication.yml
summary_line: none/oauth2/openIdConnect · 1 scheme
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
