---
api_key_in:
- header
api_specs:
- filename: northbeam-orders-v2-openapi.yml
  format: yaml
  label: Northbeam Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-orders-v2-openapi.yml
- filename: northbeam-spend-v1-openapi.yml
  format: yaml
  label: Northbeam Spend API
  slug: spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-spend-v1-openapi.yml
- filename: northbeam-data-export-v1-openapi.yml
  format: yaml
  label: Northbeam Data Export API
  slug: data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-data-export-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Northbeam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Northbeam secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Northbeam
provider_slug: northbeam
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/northbeam-data-export-v1-openapi.yml
  - openapi/northbeam-orders-v1-openapi.yml
  - openapi/northbeam-orders-v2-openapi.yml
  - openapi/northbeam-spend-v1-openapi.yml
  type: apiKey
- in: header
  name: client_id
  parameter: Data-Client-ID
  sources:
  - openapi/northbeam-data-export-v1-openapi.yml
  - openapi/northbeam-orders-v1-openapi.yml
  - openapi/northbeam-orders-v2-openapi.yml
  - openapi/northbeam-spend-v1-openapi.yml
  type: apiKey
slug: northbeam-authentication
source_filename: northbeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/northbeam-data-export-v1-openapi.yml, openapi/northbeam-orders-v1-openapi.yml,\n  openapi/northbeam-orders-v2-openapi.yml, openapi/northbeam-spend-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/northbeam-data-export-v1-openapi.yml\n  - openapi/northbeam-orders-v1-openapi.yml\n  - openapi/northbeam-orders-v2-openapi.yml\n  - openapi/northbeam-spend-v1-openapi.yml\n- name: client_id\n  type: apiKey\n  in: header\n  parameter: Data-Client-ID\n  sources:\n  - openapi/northbeam-data-export-v1-openapi.yml\n  - openapi/northbeam-orders-v1-openapi.yml\n  - openapi/northbeam-orders-v2-openapi.yml\n  - openapi/northbeam-spend-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/authentication/northbeam-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Marketing Attribution
- Multi-Touch Attribution
- E-Commerce
- ROAS
- Media Mix Modeling
- Creative Analytics
- Performance Marketing
- Advertising
- Marketing Analytics
- Agents
---
