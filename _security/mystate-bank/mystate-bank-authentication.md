---
api_key_in: []
api_specs:
- filename: mystate-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MyState Bank CDR Product Reference Data API
  slug: mystate-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-cds-banking-products-openapi.yml
- filename: mystate-bank-cds-banking-openapi.yml
  format: yaml
  label: MyState Bank CDR Accounts & Balances API
  slug: mystate-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-cds-banking-openapi.yml
- filename: mystate-bank-cds-banking-openapi.yml
  format: yaml
  label: MyState Bank CDR Transactions API
  slug: mystate-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-cds-banking-openapi.yml
- filename: mystate-bank-cds-banking-openapi.yml
  format: yaml
  label: MyState Bank CDR Direct Debits & Scheduled Payments API
  slug: mystate-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-cds-banking-openapi.yml
- filename: mystate-bank-cds-banking-openapi.yml
  format: yaml
  label: MyState Bank CDR Payees API
  slug: mystate-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-cds-banking-openapi.yml
auth_types:
- none
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Mystate Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MyState Bank secures its APIs with none, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MyState Bank
provider_slug: mystate-bank
scheme_count: 3
schemes:
- applies_to: PRD (products) endpoints
  name: none
  type: none
- flows:
  - detail: Consent is captured in the data holder's authorisation UI; the ADR receives an authorization code exchanged for an access/refresh token scoped to the consented data clusters (e.g. bank:accounts.basic:read, bank:accounts.detail:read, bank:transactions:read, bank:payees:read, bank:regular_payments:read).
    flow: authorizationCode
  name: CDR OAuth2 (FAPI)
  scheme_notes: 'OAuth 2.0 authorization-code flow hardened to the FAPI profile: Pushed Authorization Requests (PAR, RFC 9126), OIDC hybrid/JARM authorization responses, private_key_jwt client authentication, PKCE, and request-object signing. Tokens are sender-constrained.'
  type: oauth2
- name: Mutual TLS
  scheme_notes: All token and resource calls are made over mutually-authenticated TLS (RFC 8705) using CDR-issued transport certificates; access tokens are certificate-bound (sender-constrained).
  type: mutualTLS
slug: mystate-bank-authentication
source_filename: mystate-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Consumer Data Standards (CDS) Information Security profile\n  https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  and MyState Bank Open Banking help\n  https://mystate.com.au/help-centre/open-banking-help/\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types:\n  - none\n  - oauth2\n  - mutualTLS\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Two distinct surfaces. The public Product Reference Data (PRD) API is\n    UNAUTHENTICATED. Every consumer-authorised banking endpoint (accounts,\n    balances, transactions, direct-debits, scheduled-payments, payees) is\n    protected by the CDR accredited-data-recipient (ADR) security model — the\n    FAPI-based CDS Information Security profile — not by an API key. The harvested\n    DSB OpenAPI declares no securitySchemes because CDR authorisation is defined\n    out-of-band at the standards\
  \ level.\nsurfaces:\n- name: Product Reference Data (public)\n  api: openapi/mystate-bank-cds-banking-products-openapi.yml\n  auth: none\n  detail: >-\n    GET /banking/products and GET /banking/products/{productId} are openly\n    callable with no credential. Only the x-v version header is required.\n- name: Consumer data sharing (authorised)\n  api: openapi/mystate-bank-cds-banking-openapi.yml\n  auth: oauth2 + mutualTLS\n  profile: CDR / FAPI (Consumer Data Standards Information Security profile)\n  detail: >-\n    Access is restricted to Accredited Data Recipients (ADRs) acting on an\n    explicit, revocable consumer consent. Callers must be onboarded to the CDR\n    Register and present a valid access token bound to that consent.\nschemes:\n- name: none\n  type: none\n  applies_to: PRD (products) endpoints\n- name: CDR OAuth2 (FAPI)\n  type: oauth2\n  scheme_notes: >-\n    OAuth 2.0 authorization-code flow hardened to the FAPI profile: Pushed\n    Authorization Requests (PAR, RFC\
  \ 9126), OIDC hybrid/JARM authorization\n    responses, private_key_jwt client authentication, PKCE, and request-object\n    signing. Tokens are sender-constrained.\n  flows:\n  - flow: authorizationCode\n    detail: >-\n      Consent is captured in the data holder's authorisation UI; the ADR receives\n      an authorization code exchanged for an access/refresh token scoped to the\n      consented data clusters (e.g. bank:accounts.basic:read,\n      bank:accounts.detail:read, bank:transactions:read, bank:payees:read,\n      bank:regular_payments:read).\n- name: Mutual TLS\n  type: mutualTLS\n  scheme_notes: >-\n    All token and resource calls are made over mutually-authenticated TLS\n    (RFC 8705) using CDR-issued transport certificates; access tokens are\n    certificate-bound (sender-constrained).\nrelated:\n  scopes_note: >-\n    CDR data-cluster scopes are defined by the Consumer Data Standards, not by a\n    bank-proprietary OpenAPI oauth2 flow, so no scopes/ artifact is derived;\
  \ the\n    consented clusters are listed above.\n  conventions: conventions/mystate-bank-conventions.yml\n  conformance: conformance/mystate-bank-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/authentication/mystate-bank-authentication.yml
summary_line: none/oauth2/mutualTLS · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
