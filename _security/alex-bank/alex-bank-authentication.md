---
api_key_in: []
api_specs:
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Product Reference Data API
  slug: alex-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Accounts & Balances API
  slug: alex-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Transactions API
  slug: alex-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Direct Debits & Scheduled Payments API
  slug: alex-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Payees API
  slug: alex-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Alex Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Alex Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Alex Bank
provider_slug: alex-bank
scheme_count: 2
schemes:
- endpoints:
    cdr_arrangement_revocation: https://secure.cdr.alex.com.au/arrangements/revoke
    introspection: https://secure.cdr.alex.com.au/connect/introspect
    jwks: https://public.cdr.alex.com.au/jwks
    pushed_authorization_request: https://secure.cdr.alex.com.au/connect/par
    registration: https://secure.cdr.alex.com.au/connect/register
    revocation: https://secure.cdr.alex.com.au/arrangements/revoke
    userinfo: https://secure.cdr.alex.com.au/userinfo
  fapi_profile:
    acr_values:
    - urn:cds.au:cdr:2
    id_token_signing_alg:
    - ES256
    mtls_sender_constrained_tokens: true
    pkce: S256
    pushed_authorization_requests: required
    request_object_signing_alg:
    - PS256
    response_modes:
    - jwt
    token_endpoint_auth: private_key_jwt
  flows:
  - authorizationUrl: https://public.cdr.alex.com.au/connect/authorize
    flow: authorizationCode
    tokenUrl: https://secure.cdr.alex.com.au/connect/token
  - flow: clientCredentials
    tokenUrl: https://secure.cdr.alex.com.au/connect/token
  issuer: https://public.cdr.alex.com.au
  name: CDR-OAuth2-OIDC
  openIdConnectUrl: https://public.cdr.alex.com.au/.well-known/openid-configuration
  sources:
  - https://public.cdr.alex.com.au/.well-known/openid-configuration
  type: openIdConnect
- name: CDR-mTLS
  note: Sender-constrained (mTLS-bound) access tokens per FAPI; token endpoint and all resource calls run over the CDR mTLS host. tls_client_certificate_bound_access_tokens=true.
  sources:
  - https://public.cdr.alex.com.au/.well-known/openid-configuration
  type: mutualTLS
slug: alex-bank-authentication
source_filename: alex-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://public.cdr.alex.com.au/.well-known/openid-configuration\ndocs: https://www.alex.bank/legal/open-banking/\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  note: >-\n    Two-tier auth. (1) The public CDR Product Reference Data endpoints\n    (GET /banking/products, GET /banking/products/{productId}) are UNAUTHENTICATED\n    by design under the Consumer Data Standards - no key, token or client cert.\n    (2) All consumer-data sharing (accounts, balances, transactions, payees, direct\n    debits, scheduled payments) is gated by the CDR FAPI security profile and is\n    reachable only by ACCC-accredited data recipients.\ntiers:\n- name: Product Reference Data (public)\n  auth: none\n  scheme: none\n  applies_to:\n  - listBankingProducts\n  - getBankingProductDetail\n  base_url: https://public.cdr.alex.com.au/cds-au/v1\n\
  - name: CDR Consumer Data Sharing (accredited data recipients only)\n  auth: FAPI 2.0 / CDR security profile\n  applies_to: all authenticated banking resources\nschemes:\n- name: CDR-OAuth2-OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://public.cdr.alex.com.au/.well-known/openid-configuration\n  issuer: https://public.cdr.alex.com.au\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public.cdr.alex.com.au/connect/authorize\n    tokenUrl: https://secure.cdr.alex.com.au/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://secure.cdr.alex.com.au/connect/token\n  endpoints:\n    pushed_authorization_request: https://secure.cdr.alex.com.au/connect/par\n    introspection: https://secure.cdr.alex.com.au/connect/introspect\n    revocation: https://secure.cdr.alex.com.au/arrangements/revoke\n    userinfo: https://secure.cdr.alex.com.au/userinfo\n    registration: https://secure.cdr.alex.com.au/connect/register\n    jwks: https://public.cdr.alex.com.au/jwks\n\
  \    cdr_arrangement_revocation: https://secure.cdr.alex.com.au/arrangements/revoke\n  fapi_profile:\n    token_endpoint_auth: private_key_jwt\n    mtls_sender_constrained_tokens: true\n    pushed_authorization_requests: required\n    pkce: S256\n    request_object_signing_alg: [PS256]\n    id_token_signing_alg: [ES256]\n    response_modes: [jwt]\n    acr_values: [urn:cds.au:cdr:2]\n  sources: [https://public.cdr.alex.com.au/.well-known/openid-configuration]\n- name: CDR-mTLS\n  type: mutualTLS\n  note: >-\n    Sender-constrained (mTLS-bound) access tokens per FAPI; token endpoint and all\n    resource calls run over the CDR mTLS host. tls_client_certificate_bound_access_tokens=true.\n  sources: [https://public.cdr.alex.com.au/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/authentication/alex-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Digital Bank
- Product Reference Data
---
