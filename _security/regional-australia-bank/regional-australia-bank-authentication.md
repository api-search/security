---
api_key_in: []
api_specs:
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Product Reference Data API
  slug: regional-australia-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Accounts & Balances API
  slug: regional-australia-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Transactions API
  slug: regional-australia-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Direct Debits & Scheduled Payments API
  slug: regional-australia-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Payees API
  slug: regional-australia-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Regional Australia Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Regional Australia Bank secures its APIs with none, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Regional Australia Bank
provider_slug: regional-australia-bank
scheme_count: 3
schemes:
- description: Public Product Reference Data endpoints require no authentication. The only mandatory request header is `x-v` (endpoint version). Applies to listBankingProducts and getBankingProductDetail.
  name: PublicPRD
  sources:
  - openapi/regional-australia-bank-cds-banking-products-openapi.yml
  type: none
- description: OAuth2 Authorization Code with PKCE for consumer data sharing; scopes are the CDR banking scopes (bank:accounts.basic:read, bank:accounts.detail:read, bank:transactions:read, bank:regular_payments:read, bank:payees:read).
  name: CDR-OAuth2
  scheme: authorizationCode
  scopes_artifact: scopes/regional-australia-bank-scopes.yml
  sources:
  - openapi/regional-australia-bank-cds-banking-products-openapi.yml
  type: oauth2
- description: OpenID Connect identity layer required by the CDR security profile; issuer and discovery are published per data holder at the CDR InfoSec baseURI.
  name: CDR-OIDC
  sources:
  - openapi/regional-australia-bank-cds-banking-products-openapi.yml
  type: openIdConnect
slug: regional-australia-bank-authentication
source_filename: regional-australia-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/regional-australia-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  Two distinct surfaces. (1) The public Product Reference Data (PRD) API\n  (Get Products / Get Product Detail) is PUBLIC and UNAUTHENTICATED - no API key,\n  no token; only the required `x-v` version header. (2) The authenticated CDR\n  consumer data sharing operations use the CDR security profile: OAuth2\n  Authorization Code with PKCE, OpenID Connect, and FAPI-aligned protections\n  (mutual-TLS sender-constrained tokens, request objects, PAR). Access is limited\n  to accredited data recipients on the CDR Register. The harvested CDS spec does\n  not declare formal `components.securitySchemes`; it carries the required scopes\n  as `x-scopes` extensions per operation.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  public_surface: unauthenticated\n  oauth2_flows:\
  \ [authorizationCode]\n  oauth2_profile: CDR security profile (FAPI 1.0 Advanced-aligned)\nschemes:\n  - name: PublicPRD\n    type: none\n    description: >-\n      Public Product Reference Data endpoints require no authentication. The only\n      mandatory request header is `x-v` (endpoint version). Applies to\n      listBankingProducts and getBankingProductDetail.\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - name: CDR-OAuth2\n    type: oauth2\n    scheme: authorizationCode\n    description: >-\n      OAuth2 Authorization Code with PKCE for consumer data sharing; scopes are\n      the CDR banking scopes (bank:accounts.basic:read, bank:accounts.detail:read,\n      bank:transactions:read, bank:regular_payments:read, bank:payees:read).\n    scopes_artifact: scopes/regional-australia-bank-scopes.yml\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - name: CDR-OIDC\n    type: openIdConnect\n    description: >-\n  \
  \    OpenID Connect identity layer required by the CDR security profile; issuer\n      and discovery are published per data holder at the CDR InfoSec baseURI.\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/authentication/regional-australia-bank-authentication.yml
summary_line: none/oauth2/openIdConnect · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer-Owned
- Product Reference Data
- Mutual Bank
---
