---
api_key_in: []
api_specs:
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Product Reference Data API
  slug: bendigo-and-adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Accounts & Balances API
  slug: bendigo-and-adelaide-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Transactions API
  slug: bendigo-and-adelaide-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Direct Debits & Scheduled Payments API
  slug: bendigo-and-adelaide-bank-cds-banking-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Payees API
  slug: bendigo-and-adelaide-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-up-developer-api-openapi.json
  format: json
  label: Up Developer API (Personal Banking)
  slug: up-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-up-developer-api-openapi.json
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up Banking CDR Product Reference Data API
  slug: up-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Adelaide Bank CDR Product Reference Data API
  slug: adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bendigo And Adelaide Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bendigo and Adelaide Bank secures its APIs with none, openIdConnect, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bendigo and Adelaide Bank
provider_slug: bendigo-and-adelaide-bank
scheme_count: 3
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  name: PublicProductReferenceData
  note: Public CDR Product Reference Data endpoints require no credentials.
  type: none
- acr_values_supported:
  - urn:cds.au:cdr:2
  - urn:cds.au:cdr:3
  applies_to: authenticated CDR data-sharing surface (accredited data recipients)
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://api.up.com.au/oidc/authorize
    flow: authorizationCode
    pushed_authorization_request_endpoint: https://secure.api.up.com.au/oidc/authorize/push
    registration_endpoint: https://secure.api.up.com.au/oidc/register
    require_pushed_authorization_requests: true
    tokenUrl: https://secure.api.up.com.au/oidc/token
  - flow: clientCredentials
    tokenUrl: https://secure.api.up.com.au/oidc/token
  id_token_signing_alg_values_supported:
  - PS256
  - ES256
  issuer: https://api.up.com.au
  name: OpenIDConnect
  openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration
  request_object_signing_alg_values_supported:
  - PS256
  - ES256
  source: well-known/bendigo-and-adelaide-bank-up-openid-configuration.json
  subject_types_supported:
  - pairwise
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  token_endpoint_auth_signing_alg_values_supported:
  - PS256
  - ES256
  type: openIdConnect
- name: MutualTLS
  note: tls_client_certificate_bound_access_tokens = true. Access tokens are bound to the data recipient's client certificate (RFC 8705); the CDR data-sharing calls run over MTLS as required by the Consumer Data Standards security profile.
  type: mutualTLS
slug: bendigo-and-adelaide-bank-authentication
source_filename: bendigo-and-adelaide-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.up.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnotes: >-\n  Two distinct auth postures. (1) The PUBLIC Product Reference Data API\n  (GET /banking/products, GET /banking/products/{productId}) is UNAUTHENTICATED — the\n  OpenAPI declares no securitySchemes and the docs state \"These are public APIs and do\n  not require authentication.\" (2) The AUTHENTICATED CDR consumer data-sharing surface is\n  governed by the Consumer Data Standards security profile (FAPI 1.0 Advanced). The profile\n  below is captured verbatim from the live Up (api.up.com.au) CDR OIDC discovery document —\n  Up is a Bendigo and Adelaide Bank brand and its infosec endpoints are the readable example\n  of the group's CDR data-holder auth model.\nsummary:\n  types: [none, openIdConnect, oauth2, mutualTLS]\n  public_prd: unauthenticated\n  oauth2_flows: [authorizationCode,\
  \ clientCredentials]\n  fapi_profile: FAPI 1.0 Advanced (CDR)\nschemes:\n- name: PublicProductReferenceData\n  type: none\n  applies_to: [listBankingProducts, getBankingProductDetail]\n  note: Public CDR Product Reference Data endpoints require no credentials.\n- name: OpenIDConnect\n  type: openIdConnect\n  source: well-known/bendigo-and-adelaide-bank-up-openid-configuration.json\n  issuer: https://api.up.com.au\n  openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration\n  applies_to: authenticated CDR data-sharing surface (accredited data recipients)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.up.com.au/oidc/authorize\n    tokenUrl: https://secure.api.up.com.au/oidc/token\n    pushed_authorization_request_endpoint: https://secure.api.up.com.au/oidc/authorize/push\n    require_pushed_authorization_requests: true\n    registration_endpoint: https://secure.api.up.com.au/oidc/register\n  - flow: clientCredentials\n    tokenUrl: https://secure.api.up.com.au/oidc/token\n\
  \  token_endpoint_auth_methods_supported: [private_key_jwt]\n  token_endpoint_auth_signing_alg_values_supported: [PS256, ES256]\n  id_token_signing_alg_values_supported: [PS256, ES256]\n  request_object_signing_alg_values_supported: [PS256, ES256]\n  code_challenge_methods_supported: [S256]\n  subject_types_supported: [pairwise]\n  acr_values_supported: [urn:cds.au:cdr:2, urn:cds.au:cdr:3]\n- name: MutualTLS\n  type: mutualTLS\n  note: >-\n    tls_client_certificate_bound_access_tokens = true. Access tokens are bound to the\n    data recipient's client certificate (RFC 8705); the CDR data-sharing calls run over\n    MTLS as required by the Consumer Data Standards security profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/authentication/bendigo-and-adelaide-bank-authentication.yml
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
