---
api_key_in: []
api_specs:
- filename: suncorp-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Balances API
  slug: suncorp-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-balances-api-openapi.yml
- filename: suncorp-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Direct Debits API
  slug: suncorp-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-direct-debits-api-openapi.yml
- filename: suncorp-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Scheduled Payments API
  slug: suncorp-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: suncorp-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Transactions API
  slug: suncorp-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-transactions-api-openapi.yml
- filename: suncorp-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Accounts API
  slug: suncorp-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-accounts-api-openapi.yml
- filename: suncorp-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Payees API
  slug: suncorp-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-payees-api-openapi.yml
- filename: suncorp-bank-banking-products-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Products API
  slug: suncorp-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Suncorp Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Suncorp Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Suncorp Bank
provider_slug: suncorp-bank
scheme_count: 2
schemes:
- acr_values_supported:
  - urn:cds.au:cdr:2
  - urn:cds.au:cdr:3
  authorization_endpoint: https://id-ob.suncorpbank.com.au/authorize
  cdr_arrangement_revocation_endpoint: https://secure-id-ob.suncorpbank.com.au/arrangements/revoke
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  id_token_signing_alg_values_supported:
  - PS256
  issuer: https://id-ob.suncorpbank.com.au
  jwks_uri: https://id-ob.suncorpbank.com.au/jwks
  name: CDR OpenID Connect
  openIdConnectUrl: https://id-ob.suncorpbank.com.au/.well-known/openid-configuration
  pushed_authorization_request_endpoint: https://secure-id-ob.suncorpbank.com.au/par
  registration_endpoint: https://secure-id-ob.suncorpbank.com.au/register
  require_pushed_authorization_requests: true
  response_types_supported:
  - code id_token
  - code
  sources:
  - well-known/suncorp-bank-openid-configuration.json
  subject_types_supported:
  - pairwise
  tls_client_certificate_bound_access_tokens: true
  token_endpoint: https://secure-id-ob.suncorpbank.com.au/token
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  type: openIdConnect
- name: mutualTLS
  note: Access tokens are TLS client-certificate bound (holder-of-key), per CDR/FAPI.
  sources:
  - well-known/suncorp-bank-openid-configuration.json
  type: mutualTLS
slug: suncorp-bank-authentication
source_filename: suncorp-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://id-ob.suncorpbank.com.au/.well-known/openid-configuration (live OIDC\n  discovery, fetched 2026-07-20) + Suncorp Bank open-banking docs\ndocs: https://www.suncorpbank.com.au/help-support/open-banking.html\nsummary:\n  model: two-tier CDR (Consumer Data Right)\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in: []\n  notes: >-\n    The public Product Reference Data (PRD) API is UNAUTHENTICATED (no API key,\n    no token). All consumer-data endpoints require CDR-accredited access under a\n    FAPI 2.0 security profile.\ntiers:\n- name: Public Product Reference Data (PRD)\n  auth: none\n  scope: unauthenticated\n  hosts: [https://id-ob.suncorpbank.com.au/cds-au/v1]\n  operations: [listBankingProducts, getBankingProductDetail]\n  evidence: openapi/suncorp-bank-cds-banking-products-openapi.yml (product paths declare no security)\n-\
  \ name: CDR consumer data sharing (accredited)\n  auth: oauth2 + openIdConnect + mutualTLS\n  scope: CDR Accredited Data Recipient (ADR) only — not openly consumable\n  profile: FAPI 2.0 / CDR security profile\n  issuer: https://id-ob.suncorpbank.com.au\nschemes:\n- name: CDR OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://id-ob.suncorpbank.com.au/.well-known/openid-configuration\n  issuer: https://id-ob.suncorpbank.com.au\n  authorization_endpoint: https://id-ob.suncorpbank.com.au/authorize\n  token_endpoint: https://secure-id-ob.suncorpbank.com.au/token\n  pushed_authorization_request_endpoint: https://secure-id-ob.suncorpbank.com.au/par\n  registration_endpoint: https://secure-id-ob.suncorpbank.com.au/register\n  jwks_uri: https://id-ob.suncorpbank.com.au/jwks\n  grant_types_supported: [authorization_code, client_credentials, refresh_token]\n  response_types_supported: [\"code id_token\", \"code\"]\n  token_endpoint_auth_methods_supported: [private_key_jwt]\n  require_pushed_authorization_requests:\
  \ true\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [PS256]\n  tls_client_certificate_bound_access_tokens: true\n  acr_values_supported: [\"urn:cds.au:cdr:2\", \"urn:cds.au:cdr:3\"]\n  subject_types_supported: [pairwise]\n  cdr_arrangement_revocation_endpoint: https://secure-id-ob.suncorpbank.com.au/arrangements/revoke\n  sources: [well-known/suncorp-bank-openid-configuration.json]\n- name: mutualTLS\n  type: mutualTLS\n  note: Access tokens are TLS client-certificate bound (holder-of-key), per CDR/FAPI.\n  sources: [well-known/suncorp-bank-openid-configuration.json]\ncontact: openbanking@suncorpbank.com.au\nscopes_ref: scopes/suncorp-bank-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/authentication/suncorp-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Consumer Data Right
---
