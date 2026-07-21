---
api_key_in: []
api_specs:
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Product Reference Data API
  slug: anz-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: ANZ Plus CDR Product Reference Data API
  slug: anz-plus-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Accounts & Balances API
  slug: anz-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Transactions API
  slug: anz-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Direct Debits & Scheduled Payments API
  slug: anz-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Payees API
  slug: anz-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Anz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australia and New Zealand Banking Group (ANZ) secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
scheme_count: 4
schemes:
- applies_to:
  - openapi/anz-cds-banking-products-openapi.yml#listBankingProducts
  - openapi/anz-cds-banking-products-openapi.yml#getBankingProductDetail
  name: PublicNoAuth
  note: Public Product Reference Data; version header x-v only.
  type: none
- applies_to:
  - non-PRD CDR banking operations (accounts, transactions, payees, payments, customer)
  flows:
  - flow: authorizationCode
    note: 'OIDC Hybrid/authorization-code flow with PAR (Pushed Authorization Requests), PKCE, and request objects per the CDR security profile. Authorization and token endpoints are published per data holder via the CDR Register / OIDC discovery, not in this product spec.

      '
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced (Financial-grade API)
  scopes_ref: scopes/anz-scopes.yml
  type: oauth2
- name: CDR-OIDC
  note: OpenID Connect identity layer on top of the FAPI OAuth2 profile for the ADR consent flow.
  type: openIdConnect
- name: CDR-mTLS
  note: 'Holder-of-key mutual TLS (RFC 8705) binds access tokens to the ADR''s client certificate for all authenticated CDR resource calls; the CDS defines the MTLS server (mtls.dh.example.com placeholder in the shared spec).

    '
  type: mutualTLS
slug: anz-authentication
source_filename: anz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://www.anz.com.au/support/legal/anz-apis/\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  tiers:\n  - name: Product Reference Data (public)\n    auth: none\n    note: >\n      The public PRD endpoints (GET /banking/products and /banking/products/{productId})\n      and the CDR discovery endpoints (/discovery/status, /discovery/outages) require\n      NO authentication. Only the mandatory x-v version header is needed. Confirmed\n      live returning HTTP 200 on both the ANZ (api.anz) and ANZ Plus (cdr.apix.anz) brands.\n  - name: Consumer data sharing (CDR ADR model)\n    auth: [oauth2, openIdConnect, mutualTLS]\n    note: >\n      All non-PRD banking data (accounts, balances, transactions, direct debits,\n      scheduled/regular payments, payees, instalment plans, customer) is gated behind\n      the CDR security profile.\
  \ Access is restricted to CDR-accredited Data Recipients\n      (ADRs) acting with explicit consumer consent obtained through the CDR\n      consent/authorisation flow.\nnotes: >\n  The harvested OpenAPI is the shared DSB Consumer Data Standards contract and expresses\n  per-operation authorization requirements via the x-scopes vendor extension rather than\n  a components.securitySchemes block, so the mechanical derive-authentication.py found no\n  formal schemes. The auth model below is captured from the Consumer Data Standards\n  Security Profile (FAPI) and the ANZ Product APIs page.\nschemes:\n- name: PublicNoAuth\n  type: none\n  applies_to:\n  - openapi/anz-cds-banking-products-openapi.yml#listBankingProducts\n  - openapi/anz-cds-banking-products-openapi.yml#getBankingProductDetail\n  note: Public Product Reference Data; version header x-v only.\n- name: CDR-FAPI-OAuth2\n  type: oauth2\n  profile: FAPI 1.0 Advanced (Financial-grade API)\n  flows:\n  - flow: authorizationCode\n   \
  \ note: >\n      OIDC Hybrid/authorization-code flow with PAR (Pushed Authorization Requests),\n      PKCE, and request objects per the CDR security profile. Authorization and token\n      endpoints are published per data holder via the CDR Register / OIDC discovery,\n      not in this product spec.\n  scopes_ref: scopes/anz-scopes.yml\n  applies_to:\n  - non-PRD CDR banking operations (accounts, transactions, payees, payments, customer)\n- name: CDR-OIDC\n  type: openIdConnect\n  note: OpenID Connect identity layer on top of the FAPI OAuth2 profile for the ADR consent flow.\n- name: CDR-mTLS\n  type: mutualTLS\n  note: >\n    Holder-of-key mutual TLS (RFC 8705) binds access tokens to the ADR's client\n    certificate for all authenticated CDR resource calls; the CDS defines the MTLS\n    server (mtls.dh.example.com placeholder in the shared spec).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/authentication/anz-authentication.yml
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
