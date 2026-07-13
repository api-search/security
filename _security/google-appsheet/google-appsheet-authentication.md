---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google AppSheet API
  slug: google-appsheet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-appsheet/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Google Appsheet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google AppSheet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google AppSheet
provider_slug: google-appsheet
scheme_count: 1
schemes:
- in: header
  name: ApplicationAccessKey
  parameter: ApplicationAccessKey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: google-appsheet-authentication
source_filename: google-appsheet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApplicationAccessKey\n  type: apiKey\n  in: header\n  parameter: ApplicationAccessKey\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-appsheet/refs/heads/main/authentication/google-appsheet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Applications
- Data
- Google
- Low-Code
- No-Code
- Tables
---
