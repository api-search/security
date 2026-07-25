---
api_key_in: []
api_specs:
- filename: obie-opendata-standard.json
  format: json
  label: Paragon Bank Open Data API (OBIE standard, unverified)
  slug: paragon-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-opendata-standard.json
- filename: obie-account-info-standard.yaml
  format: yaml
  label: Paragon Bank Account and Transaction Information API (OBIE standard, unverified)
  slug: paragon-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-account-info-standard.yaml
- filename: obie-payment-initiation-standard.yaml
  format: yaml
  label: Paragon Bank Payment Initiation API (OBIE standard, unverified)
  slug: paragon-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-payment-initiation-standard.yaml
- filename: obie-confirmation-funds-standard.yaml
  format: yaml
  label: Paragon Bank Confirmation of Funds API (OBIE standard, unverified)
  slug: paragon-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-confirmation-funds-standard.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paragon Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Paragon Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Paragon Bank
provider_slug: paragon-bank
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/obie-account-info-standard.yaml
  - openapi/obie-confirmation-funds-standard.yaml
  - openapi/obie-payment-initiation-standard.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/obie-account-info-standard.yaml
  - openapi/obie-confirmation-funds-standard.yaml
  - openapi/obie-payment-initiation-standard.yaml
  type: oauth2
slug: paragon-bank-authentication
source_filename: paragon-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/obie-account-info-standard.yaml, openapi/obie-confirmation-funds-standard.yaml,\n  openapi/obie-payment-initiation-standard.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/obie-account-info-standard.yaml\n  - openapi/obie-confirmation-funds-standard.yaml\n  - openapi/obie-payment-initiation-standard.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants\
  \ to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/obie-account-info-standard.yaml\n  - openapi/obie-confirmation-funds-standard.yaml\n  - openapi/obie-payment-initiation-standard.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/authentication/paragon-bank-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial Services
- Banking
- Savings
- Mortgages
- Specialist Lender
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Account Information
---
