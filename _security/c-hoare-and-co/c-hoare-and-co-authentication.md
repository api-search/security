---
api_key_in: []
api_specs:
- filename: c-hoare-and-co-account-and-transaction-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Account and Transaction Information API
  slug: c-hoare-and-co-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml
- filename: c-hoare-and-co-payment-initiation-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Payment Initiation API
  slug: c-hoare-and-co-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-payment-initiation-api-openapi.yml
- filename: c-hoare-and-co-dynamic-client-registration-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Dynamic Client Registration API
  slug: c-hoare-and-co-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-dynamic-client-registration-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: C Hoare And Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: C. Hoare & Co. secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: C. Hoare & Co.
provider_slug: c-hoare-and-co
scheme_count: 2
schemes:
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  sources:
  - openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml
  - openapi/c-hoare-and-co-payment-initiation-api-openapi.yml
  type: oauth2
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  sources:
  - openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml
  - openapi/c-hoare-and-co-dynamic-client-registration-api-openapi.yml
  - openapi/c-hoare-and-co-payment-initiation-api-openapi.yml
  type: oauth2
slug: c-hoare-and-co-authentication
source_filename: c-hoare-and-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml, openapi/c-hoare-and-co-dynamic-client-registration-api-openapi.yml,\n  openapi/c-hoare-and-co-payment-initiation-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n  sources:\n  - openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml\n  - openapi/c-hoare-and-co-payment-initiation-api-openapi.yml\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n\
  \    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml\n  - openapi/c-hoare-and-co-dynamic-client-registration-api-openapi.yml\n  - openapi/c-hoare-and-co-payment-initiation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/authentication/c-hoare-and-co-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial Services
- Banking
- Private Bank
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
---
