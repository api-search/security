---
api_key_in: []
api_specs:
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Product Reference Data API
  slug: auswide-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Accounts & Balances API
  slug: auswide-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Transactions API
  slug: auswide-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Direct Debits & Scheduled Payments API
  slug: auswide-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Payees API
  slug: auswide-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Auswide Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auswide Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Auswide Bank
provider_slug: auswide-bank
scheme_count: 4
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: 'The Product Reference Data (PRD) endpoints (GET /banking/products, GET /banking/products/{productId}) are public and unauthenticated. Access is governed only by API version negotiation via the mandatory x-v request header (Auswide currently serves x-v 4 for the product list). No token, key, or consent is required. Confirmed live: HTTP 200 at https://api.auswidebank.com.au/openbanking/cds-au/v1/banking/products.'
  name: ProductReferenceData
  type: none
- description: 'Consumer-data endpoints (accounts, balances, transactions, direct debits, scheduled/regular payments, payees) require the CDR consent + authorization flow: OAuth2 authorization code with Pushed Authorization Requests (PAR) and PKCE, per the CDR Security Profile (FAPI-based). Not exposed for unauthenticated harvest; requires an Accredited Data Recipient (ADR).'
  flows:
  - authorizationCode
  name: CDR-OAuth2
  type: oauth2
- description: OpenID Connect underpins consumer consent and ID token issuance under the CDR Security Profile. The data holder's OIDC discovery document is published on the ADR-facing infosec baseline endpoint (not on the public PRD host; the public /.well-known/openid-configuration returned 404 on 2026-07-20).
  name: CDR-OIDC
  type: openIdConnect
- description: Consumer-data (holder) endpoints are served over mutual TLS with sender-constrained (MTLS-bound) access tokens per the CDR Security Profile.
  name: CDR-MTLS
  type: mutualTLS
slug: auswide-bank-authentication
source_filename: auswide-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.auswidebank.com.au/help/banking-support/open-banking/\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  The harvested OpenAPI (openapi/auswide-bank-cds-banking-products-openapi.yml) is\n  the shared DSB Consumer Data Standards banking contract and declares no in-spec\n  securitySchemes (authorization is defined by the CDR Security Profile, an\n  FAPI-based OAuth2/OIDC regime enforced outside the OpenAPI document). This profile\n  is derived from the CDR regime + the confirmed live behaviour of Auswide's public\n  Product Reference Data endpoint.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  public_prd_auth: none\n  consumer_data_auth: CDR FAPI 2.0 profile (OAuth2 authorization code + PAR + PKCE, OIDC, MTLS-bound tokens)\nschemes:\n- name: ProductReferenceData\n  type: none\n  description: >-\n    The Product Reference Data (PRD) endpoints\
  \ (GET /banking/products,\n    GET /banking/products/{productId}) are public and unauthenticated. Access is\n    governed only by API version negotiation via the mandatory x-v request header\n    (Auswide currently serves x-v 4 for the product list). No token, key, or\n    consent is required. Confirmed live: HTTP 200 at\n    https://api.auswidebank.com.au/openbanking/cds-au/v1/banking/products.\n  applies_to:\n  - listBankingProducts\n  - getBankingProductDetail\n- name: CDR-OAuth2\n  type: oauth2\n  description: >-\n    Consumer-data endpoints (accounts, balances, transactions, direct debits,\n    scheduled/regular payments, payees) require the CDR consent + authorization\n    flow: OAuth2 authorization code with Pushed Authorization Requests (PAR) and\n    PKCE, per the CDR Security Profile (FAPI-based). Not exposed for\n    unauthenticated harvest; requires an Accredited Data Recipient (ADR).\n  flows:\n  - authorizationCode\n- name: CDR-OIDC\n  type: openIdConnect\n  description:\
  \ >-\n    OpenID Connect underpins consumer consent and ID token issuance under the CDR\n    Security Profile. The data holder's OIDC discovery document is published on the\n    ADR-facing infosec baseline endpoint (not on the public PRD host; the public\n    /.well-known/openid-configuration returned 404 on 2026-07-20).\n- name: CDR-MTLS\n  type: mutualTLS\n  description: >-\n    Consumer-data (holder) endpoints are served over mutual TLS with\n    sender-constrained (MTLS-bound) access tokens per the CDR Security Profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/authentication/auswide-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
