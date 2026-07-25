---
api_key_in:
- header
api_specs:
- filename: idanalyzer-account-api-openapi.yml
  format: yaml
  label: ID Analyzer Account API
  slug: idanalyzer-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-account-api-openapi.yml
- filename: idanalyzer-aml-api-openapi.yml
  format: yaml
  label: ID Analyzer AML API
  slug: idanalyzer-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-aml-api-openapi.yml
- filename: idanalyzer-biometric-api-openapi.yml
  format: yaml
  label: ID Analyzer Biometric API
  slug: idanalyzer-biometric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-biometric-api-openapi.yml
- filename: idanalyzer-contract-api-openapi.yml
  format: yaml
  label: ID Analyzer Contract API
  slug: idanalyzer-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-contract-api-openapi.yml
- filename: idanalyzer-docupass-api-openapi.yml
  format: yaml
  label: ID Analyzer Docupass API
  slug: idanalyzer-docupass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-docupass-api-openapi.yml
- filename: idanalyzer-profile-api-openapi.yml
  format: yaml
  label: ID Analyzer Profile API
  slug: idanalyzer-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-profile-api-openapi.yml
- filename: idanalyzer-scanner-api-openapi.yml
  format: yaml
  label: ID Analyzer Scanner API
  slug: idanalyzer-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-scanner-api-openapi.yml
- filename: idanalyzer-transaction-api-openapi.yml
  format: yaml
  label: ID Analyzer Transaction API
  slug: idanalyzer-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-transaction-api-openapi.yml
- filename: idanalyzer-webhook-api-openapi.yml
  format: yaml
  label: ID Analyzer Webhook API
  slug: idanalyzer-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/openapi/idanalyzer-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Idanalyzer Authentication
name_suffix: Authentication
oauth_flows: []
overview: ID Analyzer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ID Analyzer
provider_slug: idanalyzer
scheme_count: 1
schemes:
- description: API key obtained from portal2.idanalyzer.com
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/idanalyzer-scanner-api-openapi.yml
  type: apiKey
slug: idanalyzer-authentication
source_filename: idanalyzer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/idanalyzer-scanner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key obtained from portal2.idanalyzer.com\n  sources:\n  - openapi/idanalyzer-scanner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idanalyzer/refs/heads/main/authentication/idanalyzer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Verification
- KYC
- AML
- Document OCR
- Biometrics
- Face Matching
- Fraud Detection
- Passport
- Driver License
- Liveness Detection
---
