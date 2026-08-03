---
api_key_in: []
api_specs:
- filename: uk-open-banking-account-info-api-openapi.yaml
  format: yaml
  label: GB Bank Account and Transaction Information API (AIS)
  slug: gb-bank-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-account-info-api-openapi.yaml
- filename: uk-open-banking-payment-initiation-api-openapi.yaml
  format: yaml
  label: GB Bank Payment Initiation API (PIS)
  slug: gb-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-payment-initiation-api-openapi.yaml
- filename: uk-open-banking-confirmation-of-funds-api-openapi.yaml
  format: yaml
  label: GB Bank Confirmation of Funds API (CBPII)
  slug: gb-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml
- filename: uk-open-banking-open-data-api-openapi.json
  format: json
  label: GB Bank Open Data API
  slug: uk-open-banking-open-data-api-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-open-data-api-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gb Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: GB Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: GB Bank
provider_slug: gb-bank
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/uk-open-banking-account-info-api-openapi.yaml
  - openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml
  - openapi/uk-open-banking-payment-initiation-api-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/uk-open-banking-account-info-api-openapi.yaml
  - openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml
  - openapi/uk-open-banking-payment-initiation-api-openapi.yaml
  type: oauth2
slug: gb-bank-authentication
source_filename: gb-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/uk-open-banking-account-info-api-openapi.yaml, openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml,\n  openapi/uk-open-banking-payment-initiation-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/uk-open-banking-account-info-api-openapi.yaml\n  - openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml\n  - openapi/uk-open-banking-payment-initiation-api-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth\
  \ flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/uk-open-banking-account-info-api-openapi.yaml\n  - openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml\n  - openapi/uk-open-banking-payment-initiation-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/authentication/gb-bank-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Savings
- Property Finance
- SME Lending
- Fintech
---
