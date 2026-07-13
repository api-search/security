---
api_key_in: []
api_specs:
- filename: the-racing-api-openapi.yml
  format: yaml
  label: The Racing API
  slug: the-racing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-racing-api/refs/heads/main/openapi/the-racing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: The Racing Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Racing API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Racing API
provider_slug: the-racing-api
scheme_count: 1
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/the-racing-api-openapi.yml
  type: http
slug: the-racing-api-authentication
source_filename: the-racing-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-racing-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/the-racing-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-racing-api/refs/heads/main/authentication/the-racing-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Horse Racing
- Sports
- Statistics
- Betting
- Analytics
---
