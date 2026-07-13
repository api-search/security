---
api_key_in:
- header
api_specs:
- filename: absentify-openapi.yml
  format: yaml
  label: Absentify API
  slug: absentify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Absentify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Absentify secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Absentify
provider_slug: absentify
scheme_count: 2
schemes:
- in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/absentify-openapi.yml
  type: apiKey
- description: API key from your absentify account settings. Requires Plus plan.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/absentify-openapi.yml
  type: apiKey
slug: absentify-authentication
source_filename: absentify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/absentify-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/absentify-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from your absentify account settings. Requires Plus plan.\n  sources:\n  - openapi/absentify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/authentication/absentify-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
---
