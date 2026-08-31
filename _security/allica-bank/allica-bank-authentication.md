---
api_key_in: []
api_specs:
- filename: allica-bank-account-access-api-openapi.yml
  format: yaml
  label: Allica Bank Account Access API
  slug: allica-bank-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-account-access-api-openapi.yml
- filename: allica-bank-accounts-api-openapi.yml
  format: yaml
  label: Allica Bank Accounts API
  slug: allica-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-accounts-api-openapi.yml
- filename: allica-bank-balances-api-openapi.yml
  format: yaml
  label: Allica Bank Balances API
  slug: allica-bank-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-balances-api-openapi.yml
- filename: allica-bank-beneficiaries-api-openapi.yml
  format: yaml
  label: Allica Bank Beneficiaries API
  slug: allica-bank-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-beneficiaries-api-openapi.yml
- filename: allica-bank-direct-debits-api-openapi.yml
  format: yaml
  label: Allica Bank Direct Debits API
  slug: allica-bank-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-direct-debits-api-openapi.yml
- filename: allica-bank-domestic-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Payments API
  slug: allica-bank-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-payments-api-openapi.yml
- filename: allica-bank-domestic-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Scheduled Payments API
  slug: allica-bank-domestic-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-scheduled-payments-api-openapi.yml
- filename: allica-bank-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Standing Orders API
  slug: allica-bank-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-standing-orders-api-openapi.yml
- filename: allica-bank-file-payments-api-openapi.yml
  format: yaml
  label: Allica Bank File Payments API
  slug: allica-bank-file-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-file-payments-api-openapi.yml
- filename: allica-bank-offers-api-openapi.yml
  format: yaml
  label: Allica Bank Offers API
  slug: allica-bank-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-offers-api-openapi.yml
- filename: allica-bank-parties-api-openapi.yml
  format: yaml
  label: Allica Bank Parties API
  slug: allica-bank-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-parties-api-openapi.yml
- filename: allica-bank-payment-details-api-openapi.yml
  format: yaml
  label: Allica Bank Payment Details API
  slug: allica-bank-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-payment-details-api-openapi.yml
- filename: allica-bank-products-api-openapi.yml
  format: yaml
  label: Allica Bank Products API
  slug: allica-bank-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-products-api-openapi.yml
- filename: allica-bank-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Scheduled Payments API
  slug: allica-bank-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-scheduled-payments-api-openapi.yml
- filename: allica-bank-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Standing Orders API
  slug: allica-bank-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-standing-orders-api-openapi.yml
- filename: allica-bank-transactions-api-openapi.yml
  format: yaml
  label: Allica Bank Transactions API
  slug: allica-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allica Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Allica Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Allica Bank
provider_slug: allica-bank
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/allica-bank-account-information-openapi.yaml
  - openapi/allica-bank-payment-initiation-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/allica-bank-account-information-openapi.yaml
  - openapi/allica-bank-payment-initiation-openapi.yaml
  type: oauth2
slug: allica-bank-authentication
source_filename: allica-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/allica-bank-account-information-openapi.yaml, openapi/allica-bank-payment-initiation-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/allica-bank-account-information-openapi.yaml\n  - openapi/allica-bank-payment-initiation-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n \
  \ - openapi/allica-bank-account-information-openapi.yaml\n  - openapi/allica-bank-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/authentication/allica-bank-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- SME
- Business Banking
- Fintech
---
