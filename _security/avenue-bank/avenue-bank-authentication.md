---
api_key_in: []
api_specs:
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Product Reference Data API
  slug: avenue-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Accounts & Balances API
  slug: avenue-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Transactions API
  slug: avenue-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Direct Debits & Scheduled Payments API
  slug: avenue-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Payees API
  slug: avenue-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Avenue Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Avenue Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Avenue Bank
provider_slug: avenue-bank
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  name: public
  note: PRD endpoints require no authentication per the standard.
  type: none
- flow: authorizationCode
  name: cdr-oauth2
  note: CDR ADR consumer-authorised access for all non-PRD families; scopes in scopes/avenue-bank-scopes.yml.
  sources:
  - openapi/avenue-bank-cds-banking-openapi.json
  type: oauth2
slug: avenue-bank-authentication
source_filename: avenue-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: The harvested OpenAPI declares no securitySchemes (it is the bare shared DSB Consumer Data Standards\n  Banking API contract). Authentication is defined by the CDR (Consumer Data Right) security profile every\n  Australian ADI data holder implements, documented here against the standard. Avenue's live registered\n  data-holder status is unverified (API host returned HTTP 403 WAF on 2026-07-21).\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  public_surface: Product Reference Data (Get Products, Get Product Detail) is public and unauthenticated.\n  protected_surface: All account/balance/transaction/payee/direct-debit/scheduled-payment/instalment families\n    require CDR consumer authorisation.\n  oauth2_flows:\n  - authorizationCode\n\
  profile:\n  standard: CDR Security Profile (FAPI 1.0 Advanced profile, AU adaptation)\n  oidc: OpenID Connect with the Hybrid/Authorization Code flow; consumer authorises data sharing.\n  par: Pushed Authorization Requests (PAR) required.\n  client_auth: private_key_jwt (asymmetric).\n  token_binding: MTLS-bound (certificate-bound) access tokens; holder-of-key.\n  consent_model: Accredited Data Recipient (ADR) requests consumer consent; sharing arrangement with lifetime\n    and scopes.\n  request_headers:\n  - x-v\n  - x-min-v\n  - x-fapi-interaction-id\n  - x-fapi-auth-date\n  - x-fapi-customer-ip-address\n  - x-cds-client-headers\nschemes:\n- name: public\n  type: none\n  applies_to:\n  - listBankingProducts\n  - getBankingProductDetail\n  note: PRD endpoints require no authentication per the standard.\n- name: cdr-oauth2\n  type: oauth2\n  flow: authorizationCode\n  note: CDR ADR consumer-authorised access for all non-PRD families; scopes in scopes/avenue-bank-scopes.yml.\n  sources:\n\
  \  - openapi/avenue-bank-cds-banking-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/authentication/avenue-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Business Banking
- Bank Guarantees
- Australia
- ADI
---
