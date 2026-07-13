---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Smokeball API
  slug: smokeball-api
  spec_type: OpenAPI
  url: https://docs.smokeball.com/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smokeball Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smokeball secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Smokeball
provider_slug: smokeball
scheme_count: 2
schemes:
- in: header
  name: api-key
  parameter: x-api-key
  sources:
  - openapi/smokeball-smokeball-api-openapi.yml
  type: apiKey
- in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/smokeball-smokeball-api-openapi.yml
  type: apiKey
slug: smokeball-authentication
source_filename: smokeball-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smokeball-smokeball-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/smokeball-smokeball-api-openapi.yml\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/smokeball-smokeball-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smokeball/refs/heads/main/authentication/smokeball-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Legal
- Law Firm
- Practice Management
- Matters
- Contacts
- Documents
- Billing
- Trust Accounting
- Time Tracking
---
