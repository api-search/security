---
api_key_in:
- header
api_specs:
- filename: rhumbix-public-api-openapi-original.json
  format: json
  label: Rhumbix Public API
  slug: rhumbix-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhumbix/refs/heads/main/openapi/rhumbix-public-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rhumbix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rhumbix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rhumbix
provider_slug: rhumbix
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/rhumbix-public-api-openapi-original.json
  type: apiKey
slug: rhumbix-authentication
source_filename: rhumbix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rhumbix-public-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/rhumbix-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhumbix/refs/heads/main/authentication/rhumbix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Applications
- Construction
- Construction Technology
- Workforce Management
- Timekeeping
- Payroll
- Field Data Collection
- Project Management
- Job Costing
- Integrations
- REST API
---
