---
api_key_in: []
api_specs:
- filename: account-info-openapi.yaml
  format: yaml
  label: UK Open Banking Read/Write API
  slug: uk-open-banking-readwrite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/OpenBankingUK/read-write-api-specs/master/dist/openapi/account-info-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Open Banking Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: UK Open Banking secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: UK Open Banking
provider_slug: open-banking-uk
scheme_count: 2
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/account-info-openapi.yaml
  - openapi/confirmation-funds-openapi.yaml
  - openapi/event-notifications-openapi.yaml
  - openapi/events-openapi.yaml
  - openapi/payment-initiation-openapi.yaml
  - openapi/vrp-openapi.yaml
  type: oauth2
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/account-info-openapi.yaml
  - openapi/confirmation-funds-openapi.yaml
  - openapi/payment-initiation-openapi.yaml
  - openapi/vrp-openapi.yaml
  type: oauth2
slug: open-banking-uk-authentication
source_filename: open-banking-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/account-info-openapi.yaml, openapi/confirmation-funds-openapi.yaml, openapi/event-notifications-openapi.yaml,\n  openapi/events-openapi.yaml, openapi/payment-initiation-openapi.yaml, openapi/vrp-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/account-info-openapi.yaml\n  - openapi/confirmation-funds-openapi.yaml\n  - openapi/event-notifications-openapi.yaml\n  - openapi/events-openapi.yaml\n  - openapi/payment-initiation-openapi.yaml\n  - openapi/vrp-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n  \
  \  tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/account-info-openapi.yaml\n  - openapi/confirmation-funds-openapi.yaml\n  - openapi/payment-initiation-openapi.yaml\n  - openapi/vrp-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-banking-uk/refs/heads/main/authentication/open-banking-uk-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Open Banking
- Financial Services
- Payments
- Account Information
- PSD2
- UK
- Banking
- Fintech
- Regulated
---
