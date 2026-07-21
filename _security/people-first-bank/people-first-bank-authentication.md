---
api_key_in: []
api_specs:
- filename: people-first-bank-cds-banking-products-openapi.yml
  format: yaml
  label: People First Bank CDR Product Reference Data API
  slug: people-first-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-cds-banking-products-openapi.yml
- filename: people-first-bank-cds-banking-products-openapi.yml
  format: yaml
  label: People First Bank CDR Accounts & Balances API
  slug: people-first-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-cds-banking-products-openapi.yml
- filename: people-first-bank-cds-banking-products-openapi.yml
  format: yaml
  label: People First Bank CDR Transactions API
  slug: people-first-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-cds-banking-products-openapi.yml
- filename: people-first-bank-cds-banking-products-openapi.yml
  format: yaml
  label: People First Bank CDR Direct Debits & Scheduled Payments API
  slug: people-first-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-cds-banking-products-openapi.yml
- filename: people-first-bank-cds-banking-products-openapi.yml
  format: yaml
  label: People First Bank CDR Payees API
  slug: people-first-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: People First Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: People First Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: People First Bank
provider_slug: people-first-bank
scheme_count: 3
schemes:
- applies_to: product-reference-data
  name: none
  sources:
  - documentation
  type: none
- name: cdr-oauth2-oidc
  note: FAPI-secured OAuth2/OIDC brokered by the CDR Register; not a self-service developer OAuth server. People First Bank publishes no client_id issuance flow outside CDR accreditation.
  scheme: authorizationCode
  sources:
  - documentation
  - dsb-infosec-profile
  type: oauth2
- name: cdr-mtls
  note: mTLS sender-constrained tokens and the MTLS data-holder base URL (mtls.dh host).
  sources:
  - openapi/people-first-bank-cds-banking-products-openapi.yml
  - dsb-infosec-profile
  type: mutualTLS
slug: people-first-bank-authentication
source_filename: people-first-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://www.peoplefirstbank.com.au/help-and-support/open-banking/open-banking-for-developers\n  + DSB Consumer Data Standards InfoSec profile + live probes (2026-07-21)\n# Two-tier authentication posture for the People First Bank CDR surface. The harvested DSB CDS\n# Banking OpenAPI (v1.36.0) declares no components.securitySchemes, so this profile is authored\n# from the bank's open-banking documentation, the DSB Consumer Data Standards InfoSec profile, and\n# confirmed live behaviour (public GET /banking/products => 200; unauthenticated GET\n# /banking/accounts => 403). No bank-proprietary OAuth endpoints are published; consumer data\n# sharing is brokered through the CDR Register, not a general-purpose developer OAuth server.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  tiers:\n    - Product Reference Data (public, unauthenticated)\n    - Consumer\
  \ data sharing (FAPI OAuth2/OIDC via the CDR accredited-data-recipient model)\ntiers:\n  - name: product-reference-data\n    surface: >-\n      /cds-au/v1/banking/products and /banking/products/{productId}\n    style: none\n    evidence: >-\n      Public and unauthenticated. Live GET https://public.openbanking.peoplefirstbank.com.au/cds-au/v1/banking/products\n      returns HTTP 200 (x-v 5) with a data.products array and no credential required.\n  - name: consumer-data-sharing\n    surface: >-\n      accounts, balances, transactions, direct-debits, scheduled-payments, payees\n    style: oauth2-oidc-fapi\n    evidence: >-\n      Unauthenticated GET https://public.openbanking.peoplefirstbank.com.au/cds-au/v1/banking/accounts\n      returns HTTP 403, confirming the surface is gated. Access is granted only to CDR-accredited\n      data recipients (ADRs) holding a consumer authorisation, per the DSB Consumer Data Standards.\n    profile:\n      standard: FAPI 1.0 Advanced (AU CDR InfoSec profile)\n\
  \      register: https://www.cdr.gov.au/  # CDR Register brokers ADR<->data-holder trust\n      client_authentication: private_key_jwt\n      request_object: pushed-authorization-requests (PAR) + JARM\n      token_binding: mutual-TLS sender-constrained access tokens\n      id_token: OpenID Connect (Hybrid / Authorization Code)\nschemes:\n  - name: none\n    type: none\n    applies_to: product-reference-data\n    sources: [documentation]\n  - name: cdr-oauth2-oidc\n    type: oauth2\n    scheme: authorizationCode\n    note: >-\n      FAPI-secured OAuth2/OIDC brokered by the CDR Register; not a self-service developer OAuth\n      server. People First Bank publishes no client_id issuance flow outside CDR accreditation.\n    sources: [documentation, dsb-infosec-profile]\n  - name: cdr-mtls\n    type: mutualTLS\n    note: mTLS sender-constrained tokens and the MTLS data-holder base URL (mtls.dh host).\n    sources: [openapi/people-first-bank-cds-banking-products-openapi.yml, dsb-infosec-profile]\n\
  docs:\n  - https://www.peoplefirstbank.com.au/help-and-support/open-banking/open-banking-for-developers\n  - https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndeveloper_contact: OpenBankingSupport@peopleschoice.com.au\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/authentication/people-first-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 3 schemes
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
