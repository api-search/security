---
api_key_in: []
api_specs:
- filename: trulioo-verifications-api-openapi.yml
  format: yaml
  label: Trulioo Verifications API
  slug: trulioo-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-verifications-api-openapi.yml
- filename: trulioo-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Configuration API
  slug: trulioo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-configuration-api-openapi.yml
- filename: trulioo-connection-api-openapi.yml
  format: yaml
  label: Trulioo Connection API
  slug: trulioo-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-connection-api-openapi.yml
- filename: trulioo-business-verification-api-openapi.yml
  format: yaml
  label: Trulioo Business Verification API
  slug: trulioo-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-verification-api-openapi.yml
- filename: trulioo-person-fraud-api-openapi.yml
  format: yaml
  label: Trulioo Person Fraud API
  slug: trulioo-person-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-person-fraud-api-openapi.yml
- filename: trulioo-document-verification-api-openapi.yml
  format: yaml
  label: Trulioo Identity Document Verification API
  slug: trulioo-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-verification-api-openapi.yml
- filename: trulioo-platform-api-openapi.yml
  format: yaml
  label: Trulioo Platform API
  slug: trulioo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-platform-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trulioo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Trulioo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Trulioo
provider_slug: trulioo
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/trulioo-business-verification-api-openapi.yml
  - openapi/trulioo-configuration-api-openapi.yml
  - openapi/trulioo-connection-api-openapi.yml
  - openapi/trulioo-document-verification-api-openapi.yml
  - openapi/trulioo-person-fraud-api-openapi.yml
  - openapi/trulioo-verifications-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  sources:
  - openapi/trulioo-business-verification-api-openapi.yml
  - openapi/trulioo-configuration-api-openapi.yml
  - openapi/trulioo-connection-api-openapi.yml
  - openapi/trulioo-document-verification-api-openapi.yml
  - openapi/trulioo-person-fraud-api-openapi.yml
  - openapi/trulioo-platform-api-openapi.yml
  - openapi/trulioo-verifications-api-openapi.yml
  type: oauth2
slug: trulioo-authentication
source_filename: trulioo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trulioo-business-verification-api-openapi.yml, openapi/trulioo-configuration-api-openapi.yml,\n  openapi/trulioo-connection-api-openapi.yml, openapi/trulioo-document-verification-api-openapi.yml,\n  openapi/trulioo-person-fraud-api-openapi.yml, openapi/trulioo-platform-api-openapi.yml, openapi/trulioo-verifications-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/trulioo-business-verification-api-openapi.yml\n  - openapi/trulioo-configuration-api-openapi.yml\n  - openapi/trulioo-connection-api-openapi.yml\n  - openapi/trulioo-document-verification-api-openapi.yml\n  - openapi/trulioo-person-fraud-api-openapi.yml\n  - openapi/trulioo-verifications-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n\
  \    scopes: 0\n  sources:\n  - openapi/trulioo-business-verification-api-openapi.yml\n  - openapi/trulioo-configuration-api-openapi.yml\n  - openapi/trulioo-connection-api-openapi.yml\n  - openapi/trulioo-document-verification-api-openapi.yml\n  - openapi/trulioo-person-fraud-api-openapi.yml\n  - openapi/trulioo-platform-api-openapi.yml\n  - openapi/trulioo-verifications-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/authentication/trulioo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity Verification
- KYC
- KYB
- AML
- Watchlist Screening
- Biometrics
- Document Verification
- Fraud Prevention
- Compliance
- Global Identity
---
