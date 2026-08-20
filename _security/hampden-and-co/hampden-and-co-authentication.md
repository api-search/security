---
api_key_in: []
api_specs:
- filename: hampden-and-co-account-information-api-openapi.yml
  format: yaml
  label: Hampden & Co Account & Transaction Information API
  slug: hampden-and-co-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-account-information-api-openapi.yml
- filename: hampden-and-co-payment-initiation-api-openapi.yml
  format: yaml
  label: Hampden & Co Payment Initiation API
  slug: hampden-and-co-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-payment-initiation-api-openapi.yml
- filename: hampden-and-co-confirmation-of-funds-api-openapi.yml
  format: yaml
  label: Hampden & Co Confirmation of Funds API
  slug: hampden-and-co-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hampden And Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Hampden & Co secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Hampden & Co
provider_slug: hampden-and-co
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/hampden-and-co-account-information-api-openapi.yml
  - openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
  - openapi/hampden-and-co-payment-initiation-api-openapi.yml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/hampden-and-co-account-information-api-openapi.yml
  - openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
  - openapi/hampden-and-co-payment-initiation-api-openapi.yml
  type: oauth2
slug: hampden-and-co-authentication
source_filename: hampden-and-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/hampden-and-co-account-information-api-openapi.yml, openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml,\n  openapi/hampden-and-co-payment-initiation-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/hampden-and-co-account-information-api-openapi.yml\n  - openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml\n  - openapi/hampden-and-co-payment-initiation-api-openapi.yml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth\
  \ flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/hampden-and-co-account-information-api-openapi.yml\n  - openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml\n  - openapi/hampden-and-co-payment-initiation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/authentication/hampden-and-co-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Banking
- Private Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
---
