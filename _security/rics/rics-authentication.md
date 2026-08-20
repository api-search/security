---
api_key_in:
- header
api_specs:
- filename: rics-digitalcommunity-api-openapi.json
  format: json
  label: RICS DigitalCommunity API
  slug: rics-digitalcommunity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-digitalcommunity-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rics Authentication
name_suffix: Authentication
oauth_flows: []
overview: RICS (Royal Institution of Chartered Surveyors) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RICS (Royal Institution of Chartered Surveyors)
provider_slug: rics
scheme_count: 1
schemes:
- description: Please enter into field the word 'Bearer' following by space and JWT
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/rics-digitalcommunity-api-openapi.json
  type: apiKey
slug: rics-authentication
source_filename: rics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/rics-digitalcommunity-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Please enter into field the word 'Bearer' following by space and JWT\n  sources:\n  - openapi/rics-digitalcommunity-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/authentication/rics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real-Estate
- United Kingdom
- Industry Body
- Valuation
- Standards
- Surveying
- Property Measurement
- Regulations
- Construction
- PropTech
---
