---
api_key_in: []
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Monument Bank Open Data API
  slug: monument-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Monument Bank Account and Transaction Information API
  slug: monument-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Monument Bank Payment Initiation API
  slug: monument-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Monument Bank Confirmation of Funds API
  slug: monument-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Monument Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Monument Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Monument Bank
provider_slug: monument-bank
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/obie-account-info-openapi.yaml
  - openapi/obie-confirmation-funds-openapi.yaml
  - openapi/obie-payment-initiation-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/obie-account-info-openapi.yaml
  - openapi/obie-confirmation-funds-openapi.yaml
  - openapi/obie-payment-initiation-openapi.yaml
  type: oauth2
slug: monument-bank-authentication
source_filename: monument-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/obie-account-info-openapi.yaml, openapi/obie-confirmation-funds-openapi.yaml,\n  openapi/obie-payment-initiation-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to\
  \ access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/authentication/monument-bank-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Savings
- Challenger Bank
- Account Information
- Payments
---
