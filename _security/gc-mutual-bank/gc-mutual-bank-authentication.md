---
api_key_in: []
api_specs:
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Product Reference Data API
  slug: gc-mutual-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Accounts & Balances API
  slug: gc-mutual-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Transactions API
  slug: gc-mutual-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Direct Debits & Scheduled Payments API
  slug: gc-mutual-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Payees API
  slug: gc-mutual-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Gc Mutual Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: G&C Mutual Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: G&C Mutual Bank
provider_slug: gc-mutual-bank
scheme_count: 3
schemes:
- applies_to:
  - GET /banking/products
  - GET /banking/products/{productId}
  description: Product Reference Data is public and unauthenticated per CDR rules. No API key, token, or client registration is required. Only the x-v version header is mandatory. Confirmed live returning HTTP 200.
  name: PublicProductReferenceData
  type: none
- applies_to: consumer data (accounts, balances, transactions, direct-debits, scheduled-payments, payees)
  description: 'Consumer data is gated to accredited data recipients via the CDR InfoSec profile: OAuth2 authorization-code + OIDC with holder-of-key mutual-TLS tokens and consumer consent. Not exercised on the public PRD surface.'
  flows:
  - features:
    - PAR (Pushed Authorization Requests)
    - request object (signed)
    - private_key_jwt or mutual-TLS client authentication
    - PKCE
    flow: authorizationCode
    grant: OIDC hybrid (code id_token)
  gating: Restricted to Accredited Data Recipients (ADRs) with active consumer consent under the CDR.
  name: CDRConsumerDataAccess
  profile: FAPI 1.0 Advanced
  type: oauth2
- applies_to: consumer data token and resource endpoints
  description: Holder-of-key sender-constrained access tokens over mutual TLS per CDR InfoSec.
  name: MutualTLS
  type: mutualTLS
slug: gc-mutual-bank-authentication
source_filename: gc-mutual-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://unity.bank/about-us/corporate-information/open-banking/\nnote: >-\n  The harvested OpenAPI (shared DSB CDS CDR Banking API) declares no\n  components.securitySchemes, so no profile could be derived mechanically. This\n  profile is documented from the DSB Consumer Data Standards, which define the\n  auth model G&C Mutual Bank implements as a CDR Data Holder.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  surfaces:\n    public_product_reference_data: none\n    consumer_data: oauth2 + openIdConnect + mutualTLS (FAPI)\nschemes:\n  - name: PublicProductReferenceData\n    type: none\n    applies_to:\n      - GET /banking/products\n      - GET /banking/products/{productId}\n    description: >-\n      Product Reference Data is public and unauthenticated per CDR rules. No API\n      key, token, or client registration is required.\
  \ Only the x-v version header\n      is mandatory. Confirmed live returning HTTP 200.\n  - name: CDRConsumerDataAccess\n    type: oauth2\n    profile: FAPI 1.0 Advanced\n    flows:\n      - flow: authorizationCode\n        grant: OIDC hybrid (code id_token)\n        features:\n          - PAR (Pushed Authorization Requests)\n          - request object (signed)\n          - private_key_jwt or mutual-TLS client authentication\n          - PKCE\n    applies_to: consumer data (accounts, balances, transactions, direct-debits, scheduled-payments, payees)\n    gating: Restricted to Accredited Data Recipients (ADRs) with active consumer consent under the CDR.\n    description: >-\n      Consumer data is gated to accredited data recipients via the CDR InfoSec\n      profile: OAuth2 authorization-code + OIDC with holder-of-key mutual-TLS\n      tokens and consumer consent. Not exercised on the public PRD surface.\n  - name: MutualTLS\n    type: mutualTLS\n    applies_to: consumer data token and\
  \ resource endpoints\n    description: Holder-of-key sender-constrained access tokens over mutual TLS per CDR InfoSec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/authentication/gc-mutual-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Mutual Bank
- Australia
---
