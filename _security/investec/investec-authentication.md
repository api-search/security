---
api_key_in: []
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Investec Account and Transaction Information API (AIS)
  slug: investec-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Investec Payment Initiation API (PIS)
  slug: investec-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Investec Confirmation of Funds API (CBPII)
  slug: investec-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Investec Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Investec secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Investec
provider_slug: investec
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
slug: investec-authentication
source_filename: investec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/obie-account-info-openapi.yaml, openapi/obie-confirmation-funds-openapi.yaml, openapi/obie-payment-initiation-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP\n    wants to access\
  \ an ASPSP resource owned by the PSU\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\ndocs: https://developer.investec.com/\nprogrammable_banking:\n  model: OAuth2 client_credentials + x-api-key\n  token_endpoint: POST https://openapi.investec.com/identity/v2/oauth2/token\n  headers:\n  - 'Authorization: Basic base64(client_id:client_secret)'\n  - 'x-api-key: <api key>'\n  - 'Content-Type: application/x-www-form-urlencoded'\n  grant_type: client_credentials\n  token_ttl_seconds: 1800\n  scopes:\n  - accounts\n  - transaction\n  note: Programmable Banking (South Africa) first-party auth; distinct from the OBIE FAPI/mTLS flows harvested\n    from the OpenAPI securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/authentication/investec-authentication.yml
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
- Specialist Bank
- Wealth Management
- FAPI
- Programmable Banking
---
