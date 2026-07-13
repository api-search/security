---
api_key_in: []
api_specs:
- filename: carbone-openapi.yml
  format: yaml
  label: Carbone Cloud HTTP API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbone/refs/heads/main/openapi/carbone-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Carbone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carbone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carbone
provider_slug: carbone
scheme_count: 1
schemes:
- description: Carbone Cloud API token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/carbone-openapi.yml
  type: http
slug: carbone-authentication
source_filename: carbone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carbone-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Carbone Cloud API token\n  sources:\n  - openapi/carbone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbone/refs/heads/main/authentication/carbone-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Generation
- PDF
- Templates
- Open Source
- Office
- DOCX
- XLSX
---
