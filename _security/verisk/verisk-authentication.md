---
api_key_in:
- header
api_specs:
- filename: verisk-insurance-analytics-openapi.yml
  format: yaml
  label: Verisk Insurance Analytics API
  slug: insurance-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-insurance-analytics-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Verisk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verisk secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verisk
provider_slug: verisk
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/verisk-insurance-analytics-openapi.yml
  type: http
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/verisk-insurance-analytics-openapi.yml
  type: apiKey
slug: verisk-authentication
source_filename: verisk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/verisk-insurance-analytics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/verisk-insurance-analytics-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/verisk-insurance-analytics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/authentication/verisk-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Insurance
- Analytics
- Risk Management
- Property Data
- Catastrophe Modeling
- Underwriting
- Claims
---
