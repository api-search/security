---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fda-regulations-fda-data-dashboard-api-api-openapi.yml
  format: yaml
  label: FDA Regulations FDA Data Dashboard API
  slug: fda-regulations-fda-data-dashboard-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/openapi/fda-regulations-fda-data-dashboard-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fda Regulations Authentication
name_suffix: Authentication
oauth_flows: []
overview: FDA Regulations secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FDA Regulations
provider_slug: fda-regulations
scheme_count: 2
schemes:
- in: header
  name: api_user
  parameter: Authorization-User
  sources:
  - openapi/fda-regulations-data-dashboard-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: Authorization-Key
  sources:
  - openapi/fda-regulations-data-dashboard-openapi.yml
  type: apiKey
slug: fda-regulations-authentication
source_filename: fda-regulations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/fda-regulations-data-dashboard-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_user\n  type: apiKey\n  in: header\n  parameter: Authorization-User\n  sources:\n  - openapi/fda-regulations-data-dashboard-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization-Key\n  sources:\n  - openapi/fda-regulations-data-dashboard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/authentication/fda-regulations-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Regulatory Compliance
- Healthcare
- Medical Devices
- Pharmaceuticals
- Food Safety
- Inspection
- Enforcement
- Federal-Government
- Public Data
- Import
---
