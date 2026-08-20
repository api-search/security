---
api_key_in: []
api_specs:
- filename: obie-opendata-openapi.json
  format: json
  label: first direct Open Data API
  slug: first-direct-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-direct/refs/heads/main/openapi/obie-opendata-openapi.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: first direct Account and Transaction Information API (AIS)
  slug: first-direct-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-direct/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: first direct Payment Initiation API (PIS)
  slug: first-direct-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-direct/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: first direct Confirmation of Funds API (CBPII)
  slug: first-direct-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-direct/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: First Direct Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: first direct secures its APIs with oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: first direct
provider_slug: first-direct
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
slug: first-direct-authentication
source_filename: first-direct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/obie-account-info-openapi.yaml, openapi/obie-confirmation-funds-openapi.yaml,\n  openapi/obie-payment-initiation-openapi.yaml\ndocs: https://develop.hsbc.com/knowledge-article/get-started-open-banking-apis\nprofile: FAPI (Financial-grade API) — UK Open Banking / OBIE Read/Write security profile\nnotes: >-\n  The OpenAPI securitySchemes declare only the oauth2 flows (placeholder authserver.example\n  URLs are the OBIE standard's examples). The real first direct / HSBC UK production model is\n  FAPI-secured and adds, beyond OAuth2/OIDC: mutual-TLS client authentication with\n  OBIE/eIDAS transport certificates, detached JWS request signing (x-jws-signature), and\n  PSD2 strong customer authentication (SCA) for the PSU authorization-code flow. Access\n  requires FCA authorisation as an AISP/PISP/CBPII and directory registration. The public\n  Open Data API requires no authentication.\nmechanisms:\n- oauth2 (TPP client_credentials\
  \ + PSU authorization_code)\n- openIdConnect\n- mutualTLS (OBIE/eIDAS transport certificates)\n- request-signing (detached JWS, x-jws-signature)\n- psd2-sca\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: TPP client credential authorisation flow with the ASPSP\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n    scopes: 1\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access\
  \ an ASPSP resource owned by the PSU\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n  - openapi/obie-confirmation-funds-openapi.yaml\n  - openapi/obie-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-direct/refs/heads/main/authentication/first-direct-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Open Data
- HSBC
- Fintech
---
