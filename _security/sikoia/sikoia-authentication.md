---
api_key_in:
- header
api_specs:
- filename: sikoia-openapi.yml
  format: yaml
  label: Sikoia API
  slug: sikoia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sikoia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sikoia secures its APIs with oauth2, http, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sikoia
provider_slug: sikoia
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: authorizationHeader
  scheme: bearer
  sources:
  - openapi/sikoia-openapi.yml
  type: http
- deprecated: true
  end_of_support: '2025-11-30'
  in: header
  name: apiKeyHeader
  parameter: apikey
  sources:
  - openapi/sikoia-openapi.yml
  type: apiKey
slug: sikoia-authentication
source_filename: sikoia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sikoia.com/docs/authentication\ndocs: https://docs.sikoia.com/docs/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  primary: oauth2 client_credentials (bearer JWT)\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: Migrated to OAuth 2.0. Legacy 'apikey' header auth deprecated; end of support 2025-11-30 (transitional\n    for pre-Jan-2024 customers).\noauth2:\n  flow: clientCredentials\n  token_url: https://oauth2.sikoia.com/token\n  token_url_staging: https://oauth2-staging.sikoia.com/token\n  scope: https://api.sikoia.com/.default\n  scope_staging: https://api-staging.sikoia.com/.default\n  token_format: JWT\n  token_expiry: 1 hour\n  client_secret_expiry: 2 years (rotatable; two secrets per application supported)\n  credential_management: https://portal.sikoia.com/Management/Applications\nschemes:\n- name: authorizationHeader\n  type: http\n  scheme: bearer\n \
  \ bearerFormat: JWT\n  sources:\n  - openapi/sikoia-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  deprecated: true\n  end_of_support: '2025-11-30'\n  sources:\n  - openapi/sikoia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/authentication/sikoia-authentication.yml
summary_line: oauth2/http/apiKey · 2 schemes
tags:
- Company
- Financial Services
- Identity Verification
- KYC
- KYB
- Onboarding
- Open Banking
- Credit
- Affordability
- Fraud & AML
- Document Verification
- RegTech
---
