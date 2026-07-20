---
api_key_in: []
api_specs:
- filename: kumospace-api-openapi.json
  format: json
  label: Kumospace API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kumospace/refs/heads/main/openapi/kumospace-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kumospace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kumospace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kumospace
provider_slug: kumospace
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: firebase
  scheme: bearer
  sources:
  - openapi/kumospace-api-openapi.json
  type: http
slug: kumospace-authentication
source_filename: kumospace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kumospace-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: firebase\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/kumospace-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kumospace/refs/heads/main/authentication/kumospace-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Virtual Office
- Remote Work
- Collaboration
- Video Conferencing
- Communications
- Real Time
- Productivity
- Meetings
- Spatial Audio
---
