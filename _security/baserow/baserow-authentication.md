---
api_key_in: []
api_specs:
- filename: schema.json
  format: json
  label: Baserow REST API
  slug: baserow-rest-api
  spec_type: OpenAPI
  url: https://api.baserow.io/api/schema.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Baserow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baserow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Baserow
provider_slug: baserow
scheme_count: 1
schemes:
- bearerFormat: Token your_token
  name: Database token
  scheme: bearer
  sources:
  - openapi/baserow-rest-api-openapi.yml
  type: http
slug: baserow-authentication
source_filename: baserow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/baserow-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Database token\n  type: http\n  scheme: bearer\n  bearerFormat: Token your_token\n  sources:\n  - openapi/baserow-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baserow/refs/heads/main/authentication/baserow-authentication.yml
summary_line: http · 1 scheme
tags:
- No-Code
- Database
- Open Source
- REST API
- Self-Hosted
- Tables
- Rows
- Automation
---
