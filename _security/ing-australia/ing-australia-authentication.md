---
api_key_in: []
api_specs:
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Product Reference Data API
  slug: ing-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Accounts & Balances API
  slug: ing-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Transactions API
  slug: ing-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Direct Debits & Scheduled Payments API
  slug: ing-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Payees API
  slug: ing-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: 'Authentication profile for ING Australia''s CDR (Open Banking) surface. The public Product Reference Data (PRD) endpoints (GET /banking/products and /banking/products/{productId}) are UNAUTHENTICATED. All other CDS Banking endpoints (accounts, balances, transactions, direct debits, scheduled payments, payees) require an authenticated CDR consumer-data-sharing session obtained through the CDR ecosystem: an Accredited Data Recipient authenticates the customer and calls the data holder under the FAPI 1.0 Advanced (Australia CDR) security profile. Derived from ING''s live OpenID Provider metadata; the OpenAPI itself declares no components.securitySchemes (it uses x-scopes extensions), so the model below is sourced from the published discovery document and the Consumer Data Standards security profile.'
kind: authentication
layout: security
method: searched
name: Ing Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: ING Australia secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: ING Australia
provider_slug: ing-australia
scheme_count: 3
schemes:
- issuer: https://id.ob.ing.com.au
  name: CDR-OIDC
  openIdConnectUrl: https://id.ob.ing.com.au/.well-known/openid-configuration
  sources:
  - well-known/ing-australia-openid-configuration.json
  type: openIdConnect
- acr_values_supported:
  - urn:cds.au:cdr:2
  - urn:cds.au:cdr:3
  cdr_arrangement_revocation_endpoint: true
  flows:
  - authorizationUrl: https://id.ob.ing.com.au/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pushed_authorization_request_endpoint: https://secure.ob.ing.com.au/par
    require_pushed_authorization_requests: true
    response_modes:
    - query
    - form_post
    - fragment
    - jwt
    response_types:
    - code id_token
    - code
    tokenUrl: https://secure.ob.ing.com.au/token
  - flow: clientCredentials
    tokenUrl: https://secure.ob.ing.com.au/token
  id_token_signing_alg_values_supported:
  - PS256
  name: CDR-OAuth2
  registration_endpoint: https://secure.ob.ing.com.au/register
  request_object_signing_alg_values_supported:
  - PS256
  sources:
  - well-known/ing-australia-openid-configuration.json
  tls_client_certificate_bound_access_tokens: true
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  type: oauth2
- description: Data-holder resource and token endpoints require mutual TLS with certificates issued under the CDR Register PKI; access tokens are certificate-bound (RFC 8705). The OpenAPI's MTLS server (mtls.dh.example.com) is the CDS placeholder for this host.
  name: CDR-mTLS
  sources:
  - openapi/ing-australia-cds-banking-products-openapi.yml
  type: mutualTLS
slug: ing-australia-authentication
source_filename: ing-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://id.ob.ing.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndescription: >-\n  Authentication profile for ING Australia's CDR (Open Banking) surface. The public\n  Product Reference Data (PRD) endpoints (GET /banking/products and\n  /banking/products/{productId}) are UNAUTHENTICATED. All other CDS Banking\n  endpoints (accounts, balances, transactions, direct debits, scheduled payments,\n  payees) require an authenticated CDR consumer-data-sharing session obtained\n  through the CDR ecosystem: an Accredited Data Recipient authenticates the customer\n  and calls the data holder under the FAPI 1.0 Advanced (Australia CDR) security\n  profile. Derived from ING's live OpenID Provider metadata; the OpenAPI itself\n  declares no components.securitySchemes (it uses x-scopes extensions), so the model\n  below is sourced from the published discovery document\
  \ and the Consumer Data\n  Standards security profile.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  profile: FAPI 1.0 Advanced (AU CDR)\n  public_endpoints: [listBankingProducts, getBankingProductDetail]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  token_endpoint_auth: [private_key_jwt]\n  par_required: true\n  mtls_bound_tokens: true\n  pkce: S256\nschemes:\n  - name: CDR-OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://id.ob.ing.com.au/.well-known/openid-configuration\n    issuer: https://id.ob.ing.com.au\n    sources: [well-known/ing-australia-openid-configuration.json]\n  - name: CDR-OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://id.ob.ing.com.au/authorize\n        tokenUrl: https://secure.ob.ing.com.au/token\n        pushed_authorization_request_endpoint: https://secure.ob.ing.com.au/par\n        require_pushed_authorization_requests: true\n        response_types: [code id_token, code]\n\
  \        response_modes: [query, form_post, fragment, jwt]\n        code_challenge_methods: [S256]\n      - flow: clientCredentials\n        tokenUrl: https://secure.ob.ing.com.au/token\n    token_endpoint_auth_methods_supported: [private_key_jwt]\n    id_token_signing_alg_values_supported: [PS256]\n    request_object_signing_alg_values_supported: [PS256]\n    acr_values_supported: [urn:cds.au:cdr:2, urn:cds.au:cdr:3]\n    tls_client_certificate_bound_access_tokens: true\n    registration_endpoint: https://secure.ob.ing.com.au/register\n    cdr_arrangement_revocation_endpoint: true\n    sources: [well-known/ing-australia-openid-configuration.json]\n  - name: CDR-mTLS\n    type: mutualTLS\n    description: >-\n      Data-holder resource and token endpoints require mutual TLS with certificates\n      issued under the CDR Register PKI; access tokens are certificate-bound\n      (RFC 8705). The OpenAPI's MTLS server (mtls.dh.example.com) is the CDS\n      placeholder for this host.\n    sources:\
  \ [openapi/ing-australia-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/authentication/ing-australia-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
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
