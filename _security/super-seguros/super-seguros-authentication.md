---
api_key_in:
- header
api_specs:
- filename: super-seguros-openapi.json
  format: json
  label: Super Studio API
  slug: super-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-seguros/refs/heads/main/openapi/super-seguros-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Super Seguros Authentication
name_suffix: Authentication
oauth_flows: []
overview: Super Seguros secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Super Seguros
provider_slug: super-seguros
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/super-seguros-openapi.json
  type: apiKey
slug: super-seguros-authentication
source_filename: super-seguros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/super-seguros-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/super-seguros-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-seguros/refs/heads/main/authentication/super-seguros-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Life Insurance
- Quotes
- Mexico
- Financial Services
- Super Studio
---
