---
api_key_in:
- header
api_specs:
- filename: boostup-openapi-original.json
  format: json
  label: Boostup Export API
  slug: boostup-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boostup/refs/heads/main/openapi/boostup-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Boostup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boostup secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boostup
provider_slug: boostup
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/boostup-openapi-original.json
  type: apiKey
slug: boostup-authentication
source_filename: boostup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/boostup-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/boostup-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boostup/refs/heads/main/authentication/boostup-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Revenue Intelligence
- Sales
- Forecasting
- Analytics
- RevOps
- Conversation Intelligence
- Data Export
- CRM
---
