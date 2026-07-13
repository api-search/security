---
api_key_in:
- header
api_specs:
- filename: apigen-apigen-openapi.yml
  format: yaml
  label: APIGen
  slug: apigen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/openapi/apigen-apigen-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apigen Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIGen secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIGen
provider_slug: apigen
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apigen-apigen-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/apigen-apigen-openapi.yml
  type: apiKey
slug: apigen-authentication
source_filename: apigen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apigen-apigen-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/apigen-apigen-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/apigen-apigen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/authentication/apigen-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
---
