---
api_key_in: []
api_specs:
- filename: johnson-and-johnson-lifescan-api-openapi.yml
  format: yaml
  label: Johnson & Johnson LifeScan API
  slug: lifescan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-and-johnson/refs/heads/main/openapi/johnson-and-johnson-lifescan-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Johnson And Johnson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Johnson & Johnson secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Johnson & Johnson
provider_slug: johnson-and-johnson
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/johnson-and-johnson-lifescan-api-openapi.yml
  type: http
slug: johnson-and-johnson-authentication
source_filename: johnson-and-johnson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/johnson-and-johnson-lifescan-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/johnson-and-johnson-lifescan-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnson-and-johnson/refs/heads/main/authentication/johnson-and-johnson-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Medical Devices
- Diabetes
- Blood Glucose
- Pharmaceuticals
- Fortune 100
---
