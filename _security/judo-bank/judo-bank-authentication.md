---
api_key_in: []
api_specs:
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Product Reference Data API
  slug: judo-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Accounts & Balances API
  slug: judo-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Transactions API
  slug: judo-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Direct Debits & Scheduled Payments API
  slug: judo-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Payees API
  slug: judo-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: Two-tier authentication model for Judo Bank's CDR Banking APIs. The public Product Reference Data (PRD) surface (GET /banking/products, /banking/products/{productId}) is entirely unauthenticated - no API key, token, or client credential is required. Every other CDR Banking resource (accounts, balances, transactions, direct debits, scheduled payments, payees) is consumer-authorized and only reachable through the CDR accredited-data-recipient (ADR) OAuth 2.0 / OpenID Connect + FAPI flow brokered by the CDR Register - there is no open self-serve developer key.
kind: authentication
layout: security
method: derived
name: Judo Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Judo Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Judo Bank
provider_slug: judo-bank
scheme_count: 4
schemes:
- applies_to:
  - GET /banking/products
  - GET /banking/products/{productId}
  name: PublicProductReferenceData
  note: Unauthenticated public product catalogue confirmed live (HTTP 200, x-v 3) at https://public.open.judo.bank/cds-au/v1. No credential required.
  type: none
- applies_to:
  - GET /banking/accounts and account detail/balances
  - GET /banking/accounts/{accountId}/transactions
  - GET /banking/accounts/{accountId}/direct-debits and scheduled payments
  - GET /banking/payees
  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  fapi: true
  flow: Consumer authorizes an accredited data recipient; the data holder (Judo Bank) authorisation server, discovered via the CDR Register, issues an authorization_code + PKCE grant. Access tokens are consumer-scoped and short-lived per the CDS security profile.
  mtls: true
  name: CDR-ADR-OAuth2
  pkce: true
  scheme: authorizationCode
  type: oauth2
- docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  name: CDR-OIDC
  note: The CDS security profile is built on OpenID Connect; identity is asserted via OIDC id_tokens in the CDR authorisation flow. OIDC discovery is not exposed on the public PRD host - authorisation-server metadata is brokered through the CDR Register, not a self-serve /.well-known/openid-configuration.
  type: openIdConnect
- name: CDR-mTLS
  note: Holder-of-key / sender-constrained access tokens over mutual TLS between the accredited data recipient and the data holder, per the FAPI 1.0 Advanced profile the CDS mandates. The OpenAPI server block itself is labelled "MTLS" (https://mtls.dh.example.com/cds-au/v1).
  type: mutualTLS
slug: judo-bank-authentication
source_filename: judo-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: >-\n  Derived from conventions/judo-bank-conventions.yml,\n  conformance/judo-bank-conformance.yml and the DSB Consumer Data Standards\n  security profile (https://consumerdatastandardsaustralia.github.io/standards/#security-profile).\n  The public Product Reference Data OpenAPI declares no securitySchemes because\n  the PRD surface is unauthenticated; the authenticated CDR data-sharing surface\n  is governed by the accredited-data-recipient (ADR) model, not a self-serve\n  developer key, so its scheme is not expressed in Judo's public spec.\ndescription: >-\n  Two-tier authentication model for Judo Bank's CDR Banking APIs. The public\n  Product Reference Data (PRD) surface (GET /banking/products,\n  /banking/products/{productId}) is entirely unauthenticated - no API key,\n  token, or client credential is required. Every other CDR Banking resource\n  (accounts, balances, transactions, direct debits, scheduled payments, payees)\n\
  \  is consumer-authorized and only reachable through the CDR\n  accredited-data-recipient (ADR) OAuth 2.0 / OpenID Connect + FAPI flow brokered\n  by the CDR Register - there is no open self-serve developer key.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_prd_auth: none\n  authenticated_surface_auth: oauth2 (authorization_code + PKCE) over OIDC, FAPI-secured, mTLS-bound\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: PublicProductReferenceData\n    type: none\n    applies_to:\n      - GET /banking/products\n      - GET /banking/products/{productId}\n    note: >-\n      Unauthenticated public product catalogue confirmed live (HTTP 200, x-v 3)\n      at https://public.open.judo.bank/cds-au/v1. No credential required.\n  - name: CDR-ADR-OAuth2\n    type: oauth2\n    scheme: authorizationCode\n    pkce: true\n    applies_to:\n      - GET /banking/accounts and account detail/balances\n      - GET /banking/accounts/{accountId}/transactions\n\
  \      - GET /banking/accounts/{accountId}/direct-debits and scheduled payments\n      - GET /banking/payees\n    flow: >-\n      Consumer authorizes an accredited data recipient; the data holder\n      (Judo Bank) authorisation server, discovered via the CDR Register, issues\n      an authorization_code + PKCE grant. Access tokens are consumer-scoped and\n      short-lived per the CDS security profile.\n    fapi: true\n    mtls: true\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  - name: CDR-OIDC\n    type: openIdConnect\n    note: >-\n      The CDS security profile is built on OpenID Connect; identity is asserted\n      via OIDC id_tokens in the CDR authorisation flow. OIDC discovery is not\n      exposed on the public PRD host - authorisation-server metadata is brokered\n      through the CDR Register, not a self-serve /.well-known/openid-configuration.\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n\
  \  - name: CDR-mTLS\n    type: mutualTLS\n    note: >-\n      Holder-of-key / sender-constrained access tokens over mutual TLS between\n      the accredited data recipient and the data holder, per the FAPI 1.0\n      Advanced profile the CDS mandates. The OpenAPI server block itself is\n      labelled \"MTLS\" (https://mtls.dh.example.com/cds-au/v1).\ndocs: https://www.judo.bank/open-banking/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/authentication/judo-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- SME Lending
- Product Reference Data
---
