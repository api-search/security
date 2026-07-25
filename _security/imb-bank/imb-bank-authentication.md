---
api_key_in: []
api_specs:
- filename: imb-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Balances API
  slug: imb-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-balances-api-openapi.yml
- filename: imb-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Direct Debits API
  slug: imb-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-direct-debits-api-openapi.yml
- filename: imb-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Scheduled Payments API
  slug: imb-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: imb-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Transactions API
  slug: imb-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-transactions-api-openapi.yml
- filename: imb-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Accounts API
  slug: imb-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-accounts-api-openapi.yml
- filename: imb-bank-banking-payees-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Payees API
  slug: imb-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-payees-api-openapi.yml
- filename: imb-bank-banking-products-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Products API
  slug: imb-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-products-api-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Imb Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: IMB Bank secures its APIs with none, openIdConnect, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: IMB Bank
provider_slug: imb-bank
scheme_count: 3
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: The GET /banking/products and GET /banking/products/{productId} endpoints are public and unauthenticated per the CDR Product Reference Data requirement; callers send only x-v (endpoint version) headers.
  name: PublicProductReferenceData
  type: none
- authorization_endpoint: https://auth.openbanking.imb.com.au/oauth2/authorize
  description: Australian Consumer Data Right authorization for member banking data. Authorization Code flow with PKCE (S256), Pushed Authorization Requests (RFC 9126, required), private_key_jwt client authentication (PS256), and TLS client-certificate-bound access tokens (RFC 8705 / FAPI). Response modes fragment and jwt.
  jwks_uri: https://openbank.openbanking.imb.com.au/oauth2/jwks
  name: CDROpenIDConnect
  openIdConnectUrl: https://openbank.openbanking.imb.com.au/.well-known/openid-configuration
  par_endpoint: https://openbank-secure.openbanking.imb.com.au/api/openbanking/push-authorization/par
  require_pushed_authorization_requests: true
  tls_client_certificate_bound_access_tokens: true
  token_endpoint: https://openbank-secure.openbanking.imb.com.au/oauth2/token
  type: openIdConnect
- description: The data-holder resource endpoints are exposed over an mTLS gateway (server url pattern https://mtls.dh.example.com/cds-au/v1 in the CDS spec); accredited data recipients present a client certificate issued under the CDR trust framework.
  name: MutualTLS
  type: mutualTLS
slug: imb-bank-authentication
source_filename: imb-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.openbanking.imb.com.au/.well-known/openid-configuration\ndocs: https://www.imb.com.au/openbanking\nnote: IMB's captured OpenAPI (the CDR Banking spec) declares no securitySchemes because\n  the public Product Reference Data (PRD) endpoints are unauthenticated. The authenticated\n  member-data surface uses the Australian CDR security profile, captured here from\n  the live OIDC discovery document.\nsummary:\n  types: [none, openIdConnect, oauth2, mutualTLS]\n  public_prd: unauthenticated\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  token_endpoint_auth: private_key_jwt\n  profile: FAPI / AU-CDR (acr urn:cds.au:cdr:2)\nschemes:\n- name: PublicProductReferenceData\n  type: none\n  description: The GET /banking/products and GET /banking/products/{productId} endpoints\n    are public and unauthenticated per the CDR Product Reference Data requirement;\n    callers send only x-v (endpoint\
  \ version) headers.\n  applies_to: [listBankingProducts, getBankingProductDetail]\n- name: CDROpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://openbank.openbanking.imb.com.au/.well-known/openid-configuration\n  description: Australian Consumer Data Right authorization for member banking data.\n    Authorization Code flow with PKCE (S256), Pushed Authorization Requests (RFC 9126,\n    required), private_key_jwt client authentication (PS256), and TLS client-certificate-bound\n    access tokens (RFC 8705 / FAPI). Response modes fragment and jwt.\n  authorization_endpoint: https://auth.openbanking.imb.com.au/oauth2/authorize\n  token_endpoint: https://openbank-secure.openbanking.imb.com.au/oauth2/token\n  par_endpoint: https://openbank-secure.openbanking.imb.com.au/api/openbanking/push-authorization/par\n  jwks_uri: https://openbank.openbanking.imb.com.au/oauth2/jwks\n  require_pushed_authorization_requests: true\n  tls_client_certificate_bound_access_tokens: true\n- name:\
  \ MutualTLS\n  type: mutualTLS\n  description: The data-holder resource endpoints are exposed over an mTLS gateway\n    (server url pattern https://mtls.dh.example.com/cds-au/v1 in the CDS spec); accredited\n    data recipients present a client certificate issued under the CDR trust framework.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/authentication/imb-bank-authentication.yml
summary_line: none/openIdConnect/oauth2/mutualTLS · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
