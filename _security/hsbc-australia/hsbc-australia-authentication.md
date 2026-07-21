---
api_key_in: []
api_specs:
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Product Reference Data API
  slug: hsbc-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Accounts & Balances API
  slug: hsbc-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Transactions API
  slug: hsbc-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: hsbc-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Payees API
  slug: hsbc-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Hsbc Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: HSBC Bank Australia secures its APIs with none, openIdConnect, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: HSBC Bank Australia
provider_slug: hsbc-australia
scheme_count: 3
schemes:
- description: Public unauthenticated CDR Product Reference Data. Requires only the x-v version header; no credentials.
  name: public-product-reference-data
  sources:
  - openapi/hsbc-australia-cds-banking-products-openapi.yml
  type: none
- description: CDR consumer data sharing, ADR-only.
  endpoints:
    authorization: https://public.ob.hsbc.com.au/cds-au/v1/oauth2/authorize
    cdr_arrangement_revocation: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/arrangements/revoke
    introspection: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/introspect
    jwks: https://public.ob.hsbc.com.au/jwks/public.jwks
    par: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/par
    registration: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/register
    revocation: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/revoke
    token: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token
    userinfo: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/userinfo
  fapi:
    acr_values:
    - urn:cds.au:cdr:2
    - urn:cds.au:cdr:3
    authorization_signed_response_alg:
    - PS256
    - ES256
    code_challenge_methods:
    - S256
    id_token_signing_alg:
    - ES256
    - PS256
    pushed_authorization_requests: required
    request_object_signing_alg:
    - ES256
    - PS256
    response_modes:
    - jwt
    response_types:
    - code
    tls_client_certificate_bound_access_tokens: true
    token_endpoint_auth_methods:
    - private_key_jwt
  name: cdr-openid-connect
  openIdConnectUrl: https://public.ob.hsbc.com.au/.well-known/openid-configuration
  sources:
  - well-known/hsbc-australia-openid-configuration.json
  type: openIdConnect
- description: Mutual TLS is required for token, introspection, registration and consumer-data endpoints on the mtls.ob.hsbc.com.au host; access tokens are certificate-bound.
  name: cdr-mtls
  sources:
  - well-known/hsbc-australia-openid-configuration.json
  type: mutualTLS
slug: hsbc-australia-authentication
source_filename: hsbc-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://public.ob.hsbc.com.au/.well-known/openid-configuration\ndocs: https://www.hsbc.com.au/help/open-banking/\nsummary:\n  types: [none, openIdConnect, oauth2, mutualTLS]\n  public_surface: unauthenticated\n  authenticated_surface: CDR security profile (FAPI)\n  oauth2_flows: [authorizationCode, clientCredentials]\nnote: |\n  HSBC Australia exposes two auth models. (1) The public Product Reference\n  Data endpoints (GET /banking/products and /banking/products/{productId})\n  are UNAUTHENTICATED by CDR design - product data contains no consumer data.\n  (2) The consumer data sharing surface (accounts, balances, transactions,\n  payees) is gated by the CDR security profile, an OpenID Connect / OAuth2\n  FAPI flow restricted to Accredited Data Recipients (ADRs). The FAPI details\n  below are read live from the OpenID Connect discovery document.\nschemes:\n- name: public-product-reference-data\n  type: none\n  description: Public\
  \ unauthenticated CDR Product Reference Data. Requires only\n    the x-v version header; no credentials.\n  sources: [openapi/hsbc-australia-cds-banking-products-openapi.yml]\n- name: cdr-openid-connect\n  type: openIdConnect\n  openIdConnectUrl: https://public.ob.hsbc.com.au/.well-known/openid-configuration\n  description: CDR consumer data sharing, ADR-only.\n  fapi:\n    pushed_authorization_requests: required\n    tls_client_certificate_bound_access_tokens: true\n    token_endpoint_auth_methods: [private_key_jwt]\n    id_token_signing_alg: [ES256, PS256]\n    request_object_signing_alg: [ES256, PS256]\n    authorization_signed_response_alg: [PS256, ES256]\n    code_challenge_methods: [S256]\n    acr_values: ['urn:cds.au:cdr:2', 'urn:cds.au:cdr:3']\n    response_types: [code]\n    response_modes: [jwt]\n  endpoints:\n    authorization: https://public.ob.hsbc.com.au/cds-au/v1/oauth2/authorize\n    token: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token\n    par: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/par\n\
  \    introspection: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/introspect\n    revocation: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/revoke\n    userinfo: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/userinfo\n    registration: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/register\n    jwks: https://public.ob.hsbc.com.au/jwks/public.jwks\n    cdr_arrangement_revocation: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/arrangements/revoke\n  sources: [well-known/hsbc-australia-openid-configuration.json]\n- name: cdr-mtls\n  type: mutualTLS\n  description: Mutual TLS is required for token, introspection, registration and\n    consumer-data endpoints on the mtls.ob.hsbc.com.au host; access tokens are\n    certificate-bound.\n  sources: [well-known/hsbc-australia-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/authentication/hsbc-australia-authentication.yml
summary_line: none/openIdConnect/oauth2/mutualTLS · 3 schemes
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
