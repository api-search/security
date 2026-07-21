---
api_key_in: []
api_specs:
- filename: commonwealth-bank-cdr-products-openapi.json
  format: json
  label: Commonwealth Bank CDR Product Reference Data API
  slug: cba-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-products-openapi.json
- filename: commonwealth-bank-cdr-accounts-openapi.json
  format: json
  label: Commonwealth Bank CDR Accounts & Balances API
  slug: cba-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-accounts-openapi.json
- filename: commonwealth-bank-cdr-transactions-openapi.json
  format: json
  label: Commonwealth Bank CDR Transactions API
  slug: cba-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-transactions-openapi.json
- filename: commonwealth-bank-cdr-regular-payments-openapi.json
  format: json
  label: Commonwealth Bank CDR Direct Debits & Scheduled Payments API
  slug: cba-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-regular-payments-openapi.json
- filename: commonwealth-bank-cdr-payees-openapi.json
  format: json
  label: Commonwealth Bank CDR Payees API
  slug: cba-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-payees-openapi.json
- filename: commonwealth-bank-cdr-customer-openapi.json
  format: json
  label: Commonwealth Bank CDR Customer API
  slug: cba-cdr-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-customer-openapi.json
- filename: commonwealth-bank-cds-banking-openapi.json
  format: json
  label: Commonwealth Bank CDR Banking API (DSB Consumer Data Standards)
  slug: cba-cds-banking-standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cds-banking-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
- none
description: ''
kind: authentication
layout: security
method: searched
name: Commonwealth Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Commonwealth Bank secures its APIs with oauth2, openIdConnect, mutualTLS, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
scheme_count: 4
schemes:
- applies_to:
  - Products/PRD
  name: cdr-public-prd
  note: Unauthenticated public product reference data; x-v header required.
  type: none
- client_authentication:
  - private_key_jwt
  - tls_client_auth
  consent: CDR consumer consent / authorisation via the Data Holder consent flow
  description: CDR ADR authorization_code flow with OIDC Hybrid, PAR (RFC 9126) and request objects, as mandated by the CDR Security Profile (FAPI 1.0 Advanced). Access tokens are sender-constrained (mTLS, RFC 8705).
  flow: authorizationCode
  name: cdr-adr-oauth2
  sender_constrained: mtls
  type: oauth2
- description: The Data Holder acts as an OpenID Provider; ADRs discover endpoints (issuer, authorization, token, PAR, JWKS) via CDR OIDC discovery and register via dynamic client registration (DCR).
  name: cdr-oidc
  type: openIdConnect
- description: Mutual-TLS at the token and resource endpoints; holder-of-key tokens.
  name: cdr-mtls
  type: mutualTLS
slug: commonwealth-bank-authentication
source_filename: commonwealth-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  CommBank developer portal (Open Banking / CDR) + Consumer Data Standards\n  Australia CDR Information Security Profile (FAPI 1.0 Advanced). The harvested\n  Swagger 2.0 / OpenAPI specs declare no securitySchemes, so this profile is\n  authored from the CDR standard the specs implement.\ndocs: https://www.commbank.com.au/banking/open-banking.html\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS, none]\n  oauth2_flows: [authorizationCode]\n  public_surface: >-\n    The CDR Product Reference Data (PRD) surface (GET /banking/products,\n    /banking/products/{productId}) is PUBLIC and UNAUTHENTICATED at\n    api.commbank.com.au/public/cds-au/v1 — only an x-v version header is required.\n  authorized_surface: >-\n    All other CDR Banking endpoints (accounts, balances, transactions, direct\n    debits, scheduled payments, payees, common customer) on\n    secure.api.commbank.com.au require an Accredited Data Recipient (ADR)\
  \ access\n    token issued under explicit consumer consent.\nschemes:\n  - name: cdr-public-prd\n    type: none\n    applies_to: [Products/PRD]\n    note: Unauthenticated public product reference data; x-v header required.\n  - name: cdr-adr-oauth2\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      CDR ADR authorization_code flow with OIDC Hybrid, PAR (RFC 9126) and\n      request objects, as mandated by the CDR Security Profile (FAPI 1.0\n      Advanced). Access tokens are sender-constrained (mTLS, RFC 8705).\n    client_authentication: [private_key_jwt, tls_client_auth]\n    sender_constrained: mtls\n    consent: CDR consumer consent / authorisation via the Data Holder consent flow\n  - name: cdr-oidc\n    type: openIdConnect\n    description: >-\n      The Data Holder acts as an OpenID Provider; ADRs discover endpoints (issuer,\n      authorization, token, PAR, JWKS) via CDR OIDC discovery and register via\n      dynamic client registration (DCR).\n  - name:\
  \ cdr-mtls\n    type: mutualTLS\n    description: Mutual-TLS at the token and resource endpoints; holder-of-key tokens.\nstandards:\n  - FAPI 1.0 Advanced (CDR Security Profile)\n  - OAuth 2.0 (RFC 6749) authorization_code\n  - OpenID Connect Core + Discovery\n  - RFC 9126 Pushed Authorization Requests (PAR)\n  - RFC 8705 mutual-TLS client auth and sender-constrained tokens\nnotes: >-\n  CommBank's business API catalogue (Fast Payment, NameCheck, PayTo) and the\n  merchant Payment Gateway also document OAuth 2.0 but their specs are\n  partner-gated and not wired here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/authentication/commonwealth-bank-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS/none · 4 schemes
tags:
- Financial
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
---
