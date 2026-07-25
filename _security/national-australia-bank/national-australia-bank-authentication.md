---
api_key_in: []
api_specs:
- filename: national-australia-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Account Balances API
  slug: national-australia-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-account-balances-api-openapi.yml
- filename: national-australia-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Account Direct Debits API
  slug: national-australia-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-account-direct-debits-api-openapi.yml
- filename: national-australia-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Account Scheduled Payments API
  slug: national-australia-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: national-australia-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Account Transactions API
  slug: national-australia-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-account-transactions-api-openapi.yml
- filename: national-australia-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Accounts API
  slug: national-australia-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-accounts-api-openapi.yml
- filename: national-australia-bank-banking-payees-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Payees API
  slug: national-australia-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-payees-api-openapi.yml
- filename: national-australia-bank-banking-products-api-openapi.yml
  format: yaml
  label: National Australia Bank Banking Products API
  slug: national-australia-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: National Australia Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: National Australia Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: National Australia Bank
provider_slug: national-australia-bank
scheme_count: 0
schemes: []
slug: national-australia-bank-authentication
source_filename: national-australia-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.api.nab.com.au/.well-known/openid-configuration\n# The captured OpenAPI declares NO components.securitySchemes: the public Product\n# Reference Data (PRD) endpoints are intentionally unauthenticated per CDR rules.\n# The broader CDS consumer-data-sharing surface is governed by NAB's live CDR\n# identity provider, whose OIDC discovery document (searched) confirms the profile\n# below: FAPI 1.0 Advanced, OAuth2 authorization_code with mandatory PAR + PKCE,\n# private_key_jwt client auth, mTLS-bound (certificate-constrained) access tokens.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\nsurfaces:\n  - name: Product Reference Data (public)\n    auth: none\n    note: GET /banking/products and /banking/products/{productId} require no credentials; only the x-v version header is mandatory.\n    operations: [listBankingProducts,\
  \ getBankingProductDetail]\n  - name: Consumer data sharing (accredited)\n    auth: cdr-security-profile\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n    oidc_discovery: https://openbank.api.nab.com.au/.well-known/openid-configuration\n    issuer: https://openbank.api.nab.com.au\n    endpoints:\n      authorization: https://openbank.api.nab.com.au/v1/idp/cdr/nab/authorise\n      token: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token\n      pushed_authorization_request: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/par\n      registration: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/register\n      jwks: https://openbank.api.nab.com.au/.well-known/keyset\n      cdr_arrangement_revocation: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/arrangements/revoke\n    profile:\n      acr_values: [urn:cds.au:cdr:2]\n      grant_types: [authorization_code, refresh_token, client_credentials]\n      response_types: [code,\
  \ code id_token]\n      token_endpoint_auth_methods: [private_key_jwt]\n      require_pushed_authorization_requests: true\n      require_signed_request_object: true\n      code_challenge_methods: [S256]\n      mtls_certificate_bound_access_tokens: true\n      id_token_signing_alg: [PS256]\n      request_object_signing_alg: [ES256, PS256]\n    scopes_ref: scopes/national-australia-bank-scopes.yml\nschemes: []  # none declared in the OpenAPI; profile above sourced from live OIDC discovery\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/authentication/national-australia-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
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
