---
api_key_in:
- header
api_specs:
- filename: freshsales-openapi.yml
  format: yaml
  label: Freshsales CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freshsales Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshsales secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshsales
provider_slug: freshsales
scheme_count: 1
schemes:
- description: 'Token-based authentication header in the form

    "Authorization: Token token=YOUR_API_KEY".'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/freshsales-openapi.yml
  type: apiKey
slug: freshsales-authentication
source_filename: freshsales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshsales-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Token-based authentication header in the form\n    \"Authorization: Token token=YOUR_API_KEY\".\n  sources:\n  - openapi/freshsales-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/authentication/freshsales-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- Sales
- Contacts
- Deals
- Pipeline
- Lead Management
- Freshworks
---
