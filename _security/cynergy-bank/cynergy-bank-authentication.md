---
api_key_in: []
api_specs:
- filename: cynergy-bank-account-information-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Account & Transaction Information API (AIS)
  slug: cynergy-bank-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-account-information-obie-standard-openapi.yaml
- filename: cynergy-bank-payment-initiation-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Payment Initiation API (PIS)
  slug: cynergy-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml
- filename: cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Confirmation of Funds API (CBPII)
  slug: cynergy-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cynergy Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cynergy Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cynergy Bank
provider_slug: cynergy-bank
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/cynergy-bank-account-information-obie-standard-openapi.yaml
  - openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
  - openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/cynergy-bank-account-information-obie-standard-openapi.yaml
  - openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
  - openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml
  type: oauth2
slug: cynergy-bank-authentication
source_filename: cynergy-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/cynergy-bank-account-information-obie-standard-openapi.yaml, openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml,\n  openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/cynergy-bank-account-information-obie-standard-openapi.yaml\n  - openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml\n  - openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n\
  \    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/cynergy-bank-account-information-obie-standard-openapi.yaml\n  - openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml\n  - openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/authentication/cynergy-bank-authentication.yml
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
- Confirmation of Funds
- Specialist Lender
---
