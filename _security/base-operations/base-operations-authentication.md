---
api_key_in:
- header
api_specs:
- filename: base-operations-openapi-original.json
  format: json
  label: Base Operations Customer API
  slug: base-operations-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Base Operations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Base Operations secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Base Operations
provider_slug: base-operations
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/base-operations-openapi-original.json
  type: apiKey
slug: base-operations-authentication
source_filename: base-operations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/base-operations-openapi-original.json\ndocs: https://www.baseoperations.com/product/api\ndetail: Include your unique API key in the X-API-KEY header with each request.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/base-operations-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/authentication/base-operations-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Threat Intelligence
- Security
- Risk Management
- Physical Security
- Crime Data
- Geospatial
- Public Safety
- Risk Scoring
---
