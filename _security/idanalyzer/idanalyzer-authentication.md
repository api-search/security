---
api_key_in:
- header
api_specs:
- filename: developer.idanalyzer.com
  format: yaml
  label: ID Analyzer Scanner API
  slug: scanner-api
  spec_type: OpenAPI
  url: https://developer.idanalyzer.com
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
