---
anonymous_access: true
api_key_in: []
api_specs:
- filename: amp-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Balances API
  slug: amp-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-balances-api-openapi.yml
- filename: amp-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Direct Debits API
  slug: amp-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-direct-debits-api-openapi.yml
- filename: amp-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Scheduled Payments API
  slug: amp-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: amp-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Transactions API
  slug: amp-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-transactions-api-openapi.yml
- filename: amp-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Accounts API
  slug: amp-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-accounts-api-openapi.yml
- filename: amp-bank-banking-payees-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Payees API
  slug: amp-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-payees-api-openapi.yml
- filename: amp-bank-banking-products-api-openapi.yml
  format: yaml
  label: AMP Bank GO Banking Products API
  slug: amp-bank-go-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-products-api-openapi.yml
- filename: amp-bank-banking-products-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Products API
  slug: amp-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Amp Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMP Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AMP Bank
provider_slug: amp-bank
scheme_count: 4
schemes:
- description: Public CDR PRD endpoints require no credential; only x-v (required) and x-min-v (optional) headers.
  name: none (Product Reference Data)
  sources:
  - openapi/amp-bank-banking-products-api-openapi.yml
  type: none
- description: 'Consumer data sharing under the CDS Security Profile. Verbatim: "Data Holders MUST support FAPI 1.0 Advanced Profile [FAPI-1.0-Advanced] . Data Holders MUST support Authorization Code Flow." and "Data Holders MUST support Pushed Authorisation Requests (PAR) via the pushed authorisation endpoint according to [PAR] . Data Holders MUST support [RFC9126] (PAR) using [PKCE] ( [RFC7636] ) with S256 as the code challenge method".'
  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  flow: authorization_code
  name: cds-fapi-oauth2-oidc
  scopes_ref: scopes/amp-bank-scopes.yml
  type: oauth2
- description: 'Data recipient client authentication. Verbatim: "private_key_jwt authentication using client_credentials authorisation grant flow according to Private Key JWT Client Authentication".'
  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  name: cds-client-authentication
  type: private_key_jwt
- description: Mutual TLS client authentication and certificate-bound access tokens (RFC 8705); CDS discovery metadata requires tls_client_certificate_bound_access_tokens, "Boolean value indicating server support for mutual TLS client certificate bound access tokens."
  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  name: cds-mtls
  type: mutualTLS
slug: amp-bank-authentication
source_filename: amp-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  authenticated: partial\n  note: >-\n    AMP publishes no authentication docs of its own; as a CDR data holder its\n    API security is defined by the DSB Consumer Data Standards (CDS) Security\n    Profile, which binds every data holder. The public Product Reference Data\n    (PRD) endpoints (GET /banking/products, /banking/products/{productId}) are\n    unauthenticated - the OpenAPI in openapi/ declares no securitySchemes and\n    requires only the x-v version header. The consumer data sharing endpoints\n    (accounts, balances, transactions, direct debits, scheduled payments,\n    payees) are reachable only by accredited data recipients through the CDS\n    FAPI flow below. The OpenAPI files in this repo\
  \ declare no securitySchemes\n    for those endpoints (derive-authentication.py found 0 on 2026-10-20), so\n    the schemes below come from the CDS text, not the contract. Probe\n    2026-10-20: https://api.cdr-api.amp.com.au/.well-known/openid-configuration\n    returned 403 (not publicly readable from here).\nschemes:\n- name: none (Product Reference Data)\n  type: none\n  description: Public CDR PRD endpoints require no credential; only x-v (required) and x-min-v (optional) headers.\n  sources:\n  - openapi/amp-bank-banking-products-api-openapi.yml\n- name: cds-fapi-oauth2-oidc\n  type: oauth2\n  flow: authorization_code\n  description: >-\n    Consumer data sharing under the CDS Security Profile. Verbatim: \"Data\n    Holders MUST support FAPI 1.0 Advanced Profile [FAPI-1.0-Advanced] . Data\n    Holders MUST support Authorization Code Flow.\" and \"Data Holders MUST\n    support Pushed Authorisation Requests (PAR) via the pushed authorisation\n    endpoint according to [PAR] . Data\
  \ Holders MUST support [RFC9126] (PAR)\n    using [PKCE] ( [RFC7636] ) with S256 as the code challenge method\".\n  scopes_ref: scopes/amp-bank-scopes.yml\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n- name: cds-client-authentication\n  type: private_key_jwt\n  description: >-\n    Data recipient client authentication. Verbatim: \"private_key_jwt\n    authentication using client_credentials authorisation grant flow according\n    to Private Key JWT Client Authentication\".\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n- name: cds-mtls\n  type: mutualTLS\n  description: >-\n    Mutual TLS client authentication and certificate-bound access tokens\n    (RFC 8705); CDS discovery metadata requires tls_client_certificate_bound_access_tokens,\n    \"Boolean value indicating server support for mutual TLS client certificate\n    bound access tokens.\"\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/authentication/amp-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
