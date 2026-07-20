---
api_key_in: []
api_specs:
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Banking API
  slug: prometeo-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Account Validation API
  slug: prometeo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Cross-Border Payments API
  slug: prometeo-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Payment API
  slug: prometeo-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Identity API (CURP)
  slug: prometeo-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prometeo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prometeo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prometeo
provider_slug: prometeo
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameterName: X-API-Key
  sources:
  - openapi/prometeo-openapi.yml
  - https://docs.prometeoapi.com
  type: apiKey
slug: prometeo-authentication
source_filename: prometeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/prometeo-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameterName: X-API-Key\n  sources:\n  - openapi/prometeo-openapi.yml\n  - https://docs.prometeoapi.com\nnotes: >-\n  Every Prometeo product (Banking, Account Validation, Cross-Border, Payment,\n  Identity, Fiscal) authenticates the application with a per-account API key sent\n  in the X-API-Key request header. Keys are issued from\n  dashboard.prometeoapi.com; a mock-data sandbox key is available immediately on\n  first login. The Banking API additionally establishes a per-end-user session:\n  POST /login/ (optionally answered via /login-procedure/ for MFA) returns a\n  session `key` that is passed as a query parameter on subsequent Banking calls.\n  Prometeo documentation notes that some services may additionally require mutual\n  TLS (mTLS), with the applicable method stated per service in the technical\
  \ docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/authentication/prometeo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Banking
- Payments
- FinTech
- LatAm
- Financial Data
- Account Validation
- Cross-Border
---
