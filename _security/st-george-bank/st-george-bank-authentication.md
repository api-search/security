---
api_key_in: []
api_specs:
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Product Reference Data API
  slug: st-george-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Accounts & Balances API
  slug: st-george-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Transactions API
  slug: st-george-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Direct Debits & Scheduled Payments API
  slug: st-george-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Payees API
  slug: st-george-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: St George Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: St.George Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: St.George Bank
provider_slug: st-george-bank
scheme_count: 3
schemes:
- flows:
  - detail: Pushed Authorization Requests (PAR) + PKCE; consent captured via the Data Holder authorisation server and bound to a sharing arrangement.
    flow: authorizationCode
  name: CDR-OAuth2
  profile: FAPI 1.0 Advanced (mandated by the Consumer Data Standards)
  scopes: scopes/st-george-bank-scopes.yml
  type: oauth2
- detail: OpenID Connect identity layer; id_token + userinfo per the CDR profile.
  name: CDR-OIDC
  type: openIdConnect
- detail: Mutual-TLS sender-constrained access tokens; client authentication via private_key_jwt and/or tls_client_auth. OpenAPI servers[] declares an MTLS server (https://mtls.dh.example.com/cds-au/v1 placeholder in the shared spec).
  name: CDR-mTLS
  type: mutualTLS
slug: st-george-bank-authentication
source_filename: st-george-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  The harvested OpenAPI (openapi/st-george-bank-cds-banking-products-openapi.yml)\n  declares no securitySchemes because it is the shared DSB \"CDR Banking API\"\n  document; the authentication model is defined by Australia's Consumer Data\n  Right security profile (CDR Register + FAPI 1.0 Advanced) and confirmed in the\n  St.George CDR review. Two distinct surfaces: an unauthenticated public PRD and\n  the ADR-gated consumer-data APIs.\ndocs: https://www.stgeorge.com.au/online-services/open-banking\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  public_surface: Product Reference Data (unauthenticated)\n  gated_surface: all account / transaction / payee / payment resources\nsurfaces:\n  - name: Product Reference Data (PRD)\n    auth: none\n    detail: >-\n      GET /banking/products and GET /banking/products/{productId} are public and\n      unauthenticated.\
  \ Only the x-v version header is required. Confirmed live\n      (HTTP 200) on https://digital-api.stgeorge.com.au/cds-au/v1/banking/products.\n  - name: Consumer data sharing (CDR)\n    auth: oauth2 + openIdConnect + mutualTLS\n    detail: >-\n      All other resources require an OAuth 2.0 access token obtained through the\n      CDR consent + authorisation flow. Only CDR-accredited Data Recipients\n      (ADRs) registered on the CDR Register can obtain tokens; there is no\n      public self-serve sign-up.\nschemes:\n  - name: CDR-OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        detail: >-\n          Pushed Authorization Requests (PAR) + PKCE; consent captured via the\n          Data Holder authorisation server and bound to a sharing arrangement.\n    scopes: scopes/st-george-bank-scopes.yml\n    profile: FAPI 1.0 Advanced (mandated by the Consumer Data Standards)\n  - name: CDR-OIDC\n    type: openIdConnect\n    detail: OpenID Connect identity layer; id_token\
  \ + userinfo per the CDR profile.\n  - name: CDR-mTLS\n    type: mutualTLS\n    detail: >-\n      Mutual-TLS sender-constrained access tokens; client authentication via\n      private_key_jwt and/or tls_client_auth. OpenAPI servers[] declares an MTLS\n      server (https://mtls.dh.example.com/cds-au/v1 placeholder in the shared spec).\nclient_authentication: [private_key_jwt, tls_client_auth]\nnotes: >-\n  method: searched because the spec omits securitySchemes (shared DSB doc); the\n  model is taken from the published CDR security profile, not fabricated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/authentication/st-george-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Westpac Group
---
