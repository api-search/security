---
api_key_in:
- header
api_specs:
- filename: denim-openapi-original.json
  format: json
  label: Denim Public API
  slug: denim-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Denim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Denim secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Denim
provider_slug: denim
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/denim-openapi-original.json
  type: apiKey
slug: denim-authentication
source_filename: denim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/denim-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/denim-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/authentication/denim-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Freight
- Factoring
- Payments
- Logistics
- Trucking
- Fintech
- Back Office
---
