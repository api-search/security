---
api_key_in: []
api_specs:
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Product Reference Data API
  slug: up-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Accounts & Balances API
  slug: up-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Transactions API
  slug: up-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Direct Debits & Scheduled Payments API
  slug: up-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Payees API
  slug: up-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-openapi.json
  format: json
  label: Up Personal Banking API
  slug: up-personal-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-openapi.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Up Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Up secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Up
provider_slug: up-bank
scheme_count: 2
schemes:
- applied_globally: true
  description: 'Personal Access Token issued to an Up customer. Presented as "Authorization: Bearer <token>". Verify a token works by calling GET /util/ping (200 on success, 401 on failure).'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/up-bank-openapi.json
  type: http
- applied_globally: false
  description: CDR / FAPI OpenID Connect provider for accredited data recipients. authorization_code + client_credentials + refresh_token; PAR required; private_key_jwt; mTLS-bound (tls_client_certificate_bound_access_tokens) access tokens; PS256/ES256; PKCE S256; JARM. Scopes catalogued in scopes/up-bank-scopes.yml.
  name: cdr_oidc
  openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration
  source: https://api.up.com.au/.well-known/openid-configuration
  type: openIdConnect
slug: up-bank-authentication
source_filename: up-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/up-bank-openapi.json\ndocs: https://developer.up.com.au/#authentication\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\nnotes: >-\n  Up presents two distinct authentication surfaces. (1) The Personal Banking\n  developer API authenticates with a Personal Access Token as an HTTP Bearer\n  token (Authorization: Bearer up:yeah:xxxx), minted by the account holder in\n  the Up app or at api.up.com.au and scoped to personal (own-account) use. (2)\n  Up is an Australian Consumer Data Right (CDR) data holder, so it also runs a\n  FAPI-grade OpenID Provider (discovery at\n  https://api.up.com.au/.well-known/openid-configuration, issuer\n  https://api.up.com.au) for accredited data recipients: authorization_code +\n  client_credentials + refresh_token grants, pushed authorization requests\n  (required), private_key_jwt\
  \ client authentication, mTLS-bound access tokens,\n  PS256/ES256 signing, S256 PKCE, and JARM (response_mode=jwt). The public CDR\n  Product Reference Data endpoint (api.up.com.au/cds-au/v1/banking/products) is\n  unauthenticated by mandate.\nschemes:\n  - name: bearer_auth\n    type: http\n    scheme: bearer\n    description: >-\n      Personal Access Token issued to an Up customer. Presented as\n      \"Authorization: Bearer <token>\". Verify a token works by calling\n      GET /util/ping (200 on success, 401 on failure).\n    sources: [openapi/up-bank-openapi.json]\n    applied_globally: true\n  - name: cdr_oidc\n    type: openIdConnect\n    openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration\n    description: >-\n      CDR / FAPI OpenID Connect provider for accredited data recipients.\n      authorization_code + client_credentials + refresh_token; PAR required;\n      private_key_jwt; mTLS-bound (tls_client_certificate_bound_access_tokens)\n      access tokens;\
  \ PS256/ES256; PKCE S256; JARM. Scopes catalogued in\n      scopes/up-bank-scopes.yml.\n    source: https://api.up.com.au/.well-known/openid-configuration\n    applied_globally: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/authentication/up-bank-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Neobank
- Product Reference Data
---
