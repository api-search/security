---
api_key_in: []
api_specs:
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Product Reference Data API
  slug: bcu-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Accounts & Balances API
  slug: bcu-bank-cdr-accounts-and-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Transactions API
  slug: bcu-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Direct Debits & Scheduled Payments API
  slug: bcu-bank-cdr-direct-debits-and-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Payees API
  slug: bcu-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bcu Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BCU Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BCU Bank
provider_slug: bcu-bank
scheme_count: 0
schemes: []
slug: bcu-bank-authentication
source_filename: bcu-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/bcu-bank-cds-banking-products-openapi.yml + DSB Consumer Data Standards (FAPI/OIDC security profile)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    The CDS Banking OpenAPI does not declare formal components.securitySchemes;\n    the CDR security model is defined normatively by the DSB Consumer Data\n    Standards Security Profile rather than inline in each Data Holder spec.\n    Authentication is captured here from the standard plus the per-operation\n    x-scopes present in the spec.\nsurfaces:\n- surface: Product Reference Data (PRD)\n  authenticated: false\n  scheme: none\n  detail: >-\n    GET /banking/products and /banking/products/{productId} are public and\n    unauthenticated. Callers still send CDS protocol headers (x-v version\n    negotiation,\
  \ optional x-min-v). Confirmed live and public at\n    https://public.cdr-api.bcu.com.au/cds-au/v1/banking/products (HTTP 200).\n- surface: Consumer data sharing (authenticated banking resources)\n  authenticated: true\n  schemes:\n  - type: oauth2\n    flow: authorizationCode\n    detail: >-\n      CDR authorization-code flow with PKCE (S256) under the OIDC Hybrid/\n      authorization-code profile; access tokens are bearer tokens scoped to the\n      CDR banking scopes below. Consent is captured through the CDR consent\n      (Authorisation) flow; access is restricted to Accredited Data Recipients.\n  - type: openIdConnect\n    detail: >-\n      OpenID Connect for identity and consent, per the CDR/FAPI profile\n      (request objects, ID tokens).\n  - type: mutualTLS\n    detail: >-\n      Mutual TLS is required on the resource server (the spec's only declared\n      server is described \"MTLS\": https://mtls.dh.example.com/cds-au/v1) and for\n      client authentication (tls_client_auth\
  \ / private_key_jwt) per FAPI 1.0\n      Advanced.\n  fapi: FAPI 1.0 Advanced\n  request_headers:\n  - x-fapi-interaction-id\n  - x-fapi-auth-date\n  - x-fapi-customer-ip-address\n  - x-cds-client-headers\nscopes_ref: scopes/bcu-bank-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/authentication/bcu-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
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
