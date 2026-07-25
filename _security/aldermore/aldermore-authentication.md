---
api_key_in: []
api_specs:
- filename: aldermore-obie-open-data-openapi.json
  format: json
  label: Aldermore Open Data API (OBIE Standard)
  slug: aldermore-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-open-data-openapi.json
- filename: aldermore-obie-account-info-openapi.yaml
  format: yaml
  label: Aldermore Account & Transaction Information API (OBIE Read/Write Standard)
  slug: aldermore-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-account-info-openapi.yaml
- filename: aldermore-obie-payment-initiation-openapi.yaml
  format: yaml
  label: Aldermore Payment Initiation API (OBIE Read/Write Standard)
  slug: aldermore-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-payment-initiation-openapi.yaml
- filename: aldermore-obie-confirmation-of-funds-openapi.yaml
  format: yaml
  label: Aldermore Confirmation of Funds API (OBIE Read/Write Standard)
  slug: aldermore-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-confirmation-of-funds-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aldermore Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Aldermore Bank secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Aldermore Bank
provider_slug: aldermore
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/aldermore-obie-account-info-openapi.yaml
  - openapi/aldermore-obie-confirmation-of-funds-openapi.yaml
  - openapi/aldermore-obie-payment-initiation-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/aldermore-obie-account-info-openapi.yaml
  - openapi/aldermore-obie-confirmation-of-funds-openapi.yaml
  - openapi/aldermore-obie-payment-initiation-openapi.yaml
  type: oauth2
slug: aldermore-authentication
source_filename: aldermore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/aldermore-obie-account-info-openapi.yaml, openapi/aldermore-obie-confirmation-of-funds-openapi.yaml,\n  openapi/aldermore-obie-payment-initiation-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/aldermore-obie-account-info-openapi.yaml\n  - openapi/aldermore-obie-confirmation-of-funds-openapi.yaml\n  - openapi/aldermore-obie-payment-initiation-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the\
  \ PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/aldermore-obie-account-info-openapi.yaml\n  - openapi/aldermore-obie-confirmation-of-funds-openapi.yaml\n  - openapi/aldermore-obie-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/authentication/aldermore-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial Services
- Banking
- Savings
- Specialist Lending
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
---
