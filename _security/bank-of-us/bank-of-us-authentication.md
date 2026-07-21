---
api_key_in: []
api_specs:
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Product Reference Data API
  slug: bank-of-us-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Accounts & Balances API
  slug: bank-of-us-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Transactions API
  slug: bank-of-us-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Direct Debits & Scheduled Payments API
  slug: bank-of-us-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Payees API
  slug: bank-of-us-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bank Of Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank of us secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bank of us
provider_slug: bank-of-us
scheme_count: 4
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: 'The Product Reference Data (PRD) endpoints (GET /banking/products, GET /banking/products/{productId}) are public and unauthenticated. Access is governed only by API version negotiation via the mandatory x-v request header (Bank of us currently serves x-v 4 for the product list). No token, key, or consent is required. Confirmed live: HTTP 200 at https://api.bankofus.com.au/OpenBanking/cds-au/v1/banking/products.'
  name: ProductReferenceData
  type: none
- description: 'Consumer-data endpoints (accounts, balances, transactions, direct debits, scheduled/regular payments, payees) require the CDR consent + authorization flow: OAuth2 authorization code with Pushed Authorization Requests (PAR) and PKCE, per the CDR Security Profile (FAPI-based). Consent is brokered through Bank of us Internet Banking identity verification and a one-time password; not exposed for unauthenticated harvest and requires an Accredited Data Recipient (ADR).'
  flows:
  - authorizationCode
  name: CDR-OAuth2
  type: oauth2
- description: OpenID Connect underpins consumer consent and ID token issuance under the CDR Security Profile. The data holder's OIDC discovery document is published on the ADR-facing infosec baseline endpoint (not on the public PRD host; the public /.well-known/openid-configuration returned 403/404 on 2026-07-20).
  name: CDR-OIDC
  type: openIdConnect
- description: Consumer-data (holder) endpoints are served over mutual TLS with sender-constrained (MTLS-bound) access tokens per the CDR Security Profile.
  name: CDR-MTLS
  type: mutualTLS
slug: bank-of-us-authentication
source_filename: bank-of-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.bankofus.com.au/open-banking\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  The harvested OpenAPI (openapi/bank-of-us-cds-banking-products-openapi.yml) is\n  the shared DSB Consumer Data Standards banking contract and declares no in-spec\n  securitySchemes (authorization is defined by the CDR Security Profile, an\n  FAPI-based OAuth2/OIDC regime enforced outside the OpenAPI document). This profile\n  is derived from the CDR regime + the confirmed live behaviour of Bank of us's\n  public Product Reference Data endpoint.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  public_prd_auth: none\n  consumer_data_auth: CDR FAPI 2.0 profile (OAuth2 authorization code + PAR + PKCE, OIDC, MTLS-bound tokens)\nschemes:\n- name: ProductReferenceData\n  type: none\n  description: >-\n    The Product Reference Data (PRD) endpoints (GET /banking/products,\n\
  \    GET /banking/products/{productId}) are public and unauthenticated. Access is\n    governed only by API version negotiation via the mandatory x-v request header\n    (Bank of us currently serves x-v 4 for the product list). No token, key, or\n    consent is required. Confirmed live: HTTP 200 at\n    https://api.bankofus.com.au/OpenBanking/cds-au/v1/banking/products.\n  applies_to:\n  - listBankingProducts\n  - getBankingProductDetail\n- name: CDR-OAuth2\n  type: oauth2\n  description: >-\n    Consumer-data endpoints (accounts, balances, transactions, direct debits,\n    scheduled/regular payments, payees) require the CDR consent + authorization\n    flow: OAuth2 authorization code with Pushed Authorization Requests (PAR) and\n    PKCE, per the CDR Security Profile (FAPI-based). Consent is brokered through\n    Bank of us Internet Banking identity verification and a one-time password; not\n    exposed for unauthenticated harvest and requires an Accredited Data Recipient (ADR).\n  flows:\n\
  \  - authorizationCode\n- name: CDR-OIDC\n  type: openIdConnect\n  description: >-\n    OpenID Connect underpins consumer consent and ID token issuance under the CDR\n    Security Profile. The data holder's OIDC discovery document is published on the\n    ADR-facing infosec baseline endpoint (not on the public PRD host; the public\n    /.well-known/openid-configuration returned 403/404 on 2026-07-20).\n- name: CDR-MTLS\n  type: mutualTLS\n  description: >-\n    Consumer-data (holder) endpoints are served over mutual TLS with\n    sender-constrained (MTLS-bound) access tokens per the CDR Security Profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/authentication/bank-of-us-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Tasmania
- Mutual
- Product Reference Data
---
