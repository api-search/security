---
api_key_in: []
api_specs:
- filename: zopa-account-access-api-openapi.yml
  format: yaml
  label: zopa Account Access API
  slug: zopa-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-account-access-api-openapi.yml
- filename: zopa-accounts-api-openapi.yml
  format: yaml
  label: zopa Accounts API
  slug: zopa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-accounts-api-openapi.yml
- filename: zopa-balances-api-openapi.yml
  format: yaml
  label: zopa Balances API
  slug: zopa-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-balances-api-openapi.yml
- filename: zopa-beneficiaries-api-openapi.yml
  format: yaml
  label: zopa Beneficiaries API
  slug: zopa-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-beneficiaries-api-openapi.yml
- filename: zopa-direct-debits-api-openapi.yml
  format: yaml
  label: zopa Direct Debits API
  slug: zopa-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-direct-debits-api-openapi.yml
- filename: zopa-domestic-payments-api-openapi.yml
  format: yaml
  label: zopa Domestic Payments API
  slug: zopa-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-payments-api-openapi.yml
- filename: zopa-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Domestic Standing Orders API
  slug: zopa-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-standing-orders-api-openapi.yml
- filename: zopa-offers-api-openapi.yml
  format: yaml
  label: zopa Offers API
  slug: zopa-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-offers-api-openapi.yml
- filename: zopa-parties-api-openapi.yml
  format: yaml
  label: zopa Parties API
  slug: zopa-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-parties-api-openapi.yml
- filename: zopa-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Standing Orders API
  slug: zopa-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-standing-orders-api-openapi.yml
- filename: zopa-statements-api-openapi.yml
  format: yaml
  label: zopa Statements API
  slug: zopa-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-statements-api-openapi.yml
- filename: zopa-transactions-api-openapi.yml
  format: yaml
  label: zopa Transactions API
  slug: zopa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zopa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: zopa secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: zopa
provider_slug: zopa
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/zopa-account-info-openapi-original.yml
  - openapi/zopa-payment-initiation-openapi-original.yml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/zopa-account-info-openapi-original.yml
  - openapi/zopa-payment-initiation-openapi-original.yml
  type: oauth2
slug: zopa-authentication
source_filename: zopa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zopa-account-info-openapi-original.yml, openapi/zopa-payment-initiation-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/zopa-account-info-openapi-original.yml\n  - openapi/zopa-payment-initiation-openapi-original.yml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/zopa-account-info-openapi-original.yml\n\
  \  - openapi/zopa-payment-initiation-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/authentication/zopa-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Banking
- Fintech
- Open Banking
- PSD2
- Payments
- Account Information
- Payment Initiation
- FAPI
- United Kingdom
- Digital Bank
- Lending
---
