---
api_key_in: []
api_specs:
- filename: algbra-account-transaction-api-openapi.yml
  format: yaml
  label: Algbra Account and Transaction Information API (AIS)
  slug: algbra-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-account-transaction-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Algbra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Algbra secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Algbra
provider_slug: algbra
scheme_count: 2
schemes:
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: PSUOAuth2Security
  sources:
  - openapi/algbra-account-transaction-api-openapi.yml
  type: oauth2
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: TPPOAuth2Security
  sources:
  - openapi/algbra-account-transaction-api-openapi.yml
  type: oauth2
slug: algbra-authentication
source_filename: algbra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/algbra-account-transaction-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/algbra-account-transaction-api-openapi.yml\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/algbra-account-transaction-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/authentication/algbra-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Fintech
- Ethical Finance
- Banking as a Service
---
