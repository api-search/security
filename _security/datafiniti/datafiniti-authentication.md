---
api_key_in: []
api_specs:
- filename: datafiniti-api.yml
  format: yaml
  label: Datafiniti API
  slug: datafiniti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datafiniti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafiniti secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datafiniti
provider_slug: datafiniti
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datafiniti-api.yml
  type: http
slug: datafiniti-authentication
source_filename: datafiniti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datafiniti-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/datafiniti-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/authentication/datafiniti-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Data
- Data Aggregation
- Data as a Service
- People Data
- Product Data
- Property Data
---
