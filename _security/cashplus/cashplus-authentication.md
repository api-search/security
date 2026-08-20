---
api_key_in: []
api_specs:
- filename: cashplus-account-information-openapi.yml
  format: yaml
  label: Cashplus Account Information API
  slug: cashplus-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-account-information-openapi.yml
- filename: cashplus-payment-initiation-openapi.yml
  format: yaml
  label: Cashplus Payment Initiation API
  slug: cashplus-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-payment-initiation-openapi.yml
- filename: cashplus-confirmation-of-funds-openapi.yml
  format: yaml
  label: Cashplus Confirmation of Funds API
  slug: cashplus-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-confirmation-of-funds-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cashplus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cashplus Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cashplus Bank
provider_slug: cashplus
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/cashplus-account-information-openapi.yml
  - openapi/cashplus-confirmation-of-funds-openapi.yml
  - openapi/cashplus-payment-initiation-openapi.yml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/cashplus-account-information-openapi.yml
  - openapi/cashplus-confirmation-of-funds-openapi.yml
  - openapi/cashplus-payment-initiation-openapi.yml
  type: oauth2
slug: cashplus-authentication
source_filename: cashplus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/cashplus-account-information-openapi.yml, openapi/cashplus-confirmation-of-funds-openapi.yml,\n  openapi/cashplus-payment-initiation-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/cashplus-account-information-openapi.yml\n  - openapi/cashplus-confirmation-of-funds-openapi.yml\n  - openapi/cashplus-payment-initiation-openapi.yml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with\
  \ the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/cashplus-account-information-openapi.yml\n  - openapi/cashplus-confirmation-of-funds-openapi.yml\n  - openapi/cashplus-payment-initiation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/authentication/cashplus-authentication.yml
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
- Challenger Bank
- Business Banking
- Fintech
---
