---
api_key_in:
- header
api_specs:
- filename: findigs-client-api-openapi.yml
  format: yaml
  label: Findigs Client API
  slug: findigs-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/openapi/findigs-client-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Findigs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Findigs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Findigs
provider_slug: findigs
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/findigs-client-api-openapi.yml
  type: apiKey
slug: findigs-authentication
source_filename: findigs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/findigs-client-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/findigs-client-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/authentication/findigs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- rental-screening
- Tenant Screening
- resident-screening
- rental-application
- Underwriting
- Decisioning
- Identity Verification
- Income Verification
- Credit Check
- Background Check
- Fraud Detection
- Property Management
- Real-Estate
- PropTech
- FCRA
- Fair Housing
- Webhook
---
