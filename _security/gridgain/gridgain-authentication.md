---
api_key_in: []
api_specs:
- filename: gridgain-openapi.yml
  format: yaml
  label: GridGain 9 Management API
  slug: gridgain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridgain/refs/heads/main/openapi/gridgain-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gridgain Authentication
name_suffix: Authentication
oauth_flows: []
overview: GridGain secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GridGain
provider_slug: gridgain
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/gridgain-openapi.yml
  type: http
- name: bearerToken
  scheme: bearer
  sources:
  - openapi/gridgain-openapi.yml
  type: http
slug: gridgain-authentication
source_filename: gridgain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gridgain-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/gridgain-openapi.yml\n- name: bearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gridgain-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridgain/refs/heads/main/authentication/gridgain-authentication.yml
summary_line: http · 2 schemes
tags:
- Caching
- Data Grid
- Distributed Database
- In-Memory Computing
- Real-Time
---
