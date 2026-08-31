---
api_key_in:
- header
api_specs:
- filename: rics-azurestorage-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Azure Storage API
  slug: rics-azurestorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-azurestorage-api-openapi.yml
- filename: rics-olamerchantpost-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Ola Merchant Post API
  slug: rics-olamerchantpost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-olamerchantpost-api-openapi.yml
- filename: rics-payment-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Payment API
  slug: rics-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-payment-api-openapi.yml
- filename: rics-profile-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Profile API
  slug: rics-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-profile-api-openapi.yml
- filename: rics-regulation-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Regulation API
  slug: rics-regulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-regulation-api-openapi.yml
- filename: rics-surveywriter-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Survey Writer API
  slug: rics-surveywriter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-surveywriter-api-openapi.yml
- filename: rics-token-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Token API
  slug: rics-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-token-api-openapi.yml
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
