---
api_key_in: []
api_specs:
- filename: zopa-account-info-openapi-original.yml
  format: yaml
  label: Zopa Account & Transaction API (AIS)
  slug: zopa-account-info
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-account-info-openapi-original.yml
- filename: zopa-payment-initiation-openapi-original.yml
  format: yaml
  label: Zopa Payment Initiation API (PIS)
  slug: zopa-payment-initiation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-payment-initiation-openapi-original.yml
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
