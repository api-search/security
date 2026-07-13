---
api_key_in:
- header
api_specs:
- filename: j-quants-openapi.yml
  format: yaml
  label: J-Quants API
  slug: j-quants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: J Quants Authentication
name_suffix: Authentication
oauth_flows: []
overview: J-Quants secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: J-Quants
provider_slug: j-quants
scheme_count: 2
schemes:
- description: Bearer ID token issued via /token/auth_refresh
  in: header
  name: idToken
  parameter: Authorization
  sources:
  - openapi/j-quants-openapi.yml
  type: apiKey
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/j-quants-openapi.yml
  type: apiKey
slug: j-quants-authentication
source_filename: j-quants-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/j-quants-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: idToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer ID token issued via /token/auth_refresh\n  sources:\n  - openapi/j-quants-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/j-quants-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/authentication/j-quants-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Financial Data
- Investment
- Japan
- Stock Market
---
