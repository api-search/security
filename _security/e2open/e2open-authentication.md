---
api_key_in: []
api_specs:
- filename: inttra-ocean-execution-openapi.yml
  format: yaml
  label: INTTRA Ocean Execution API
  slug: inttra-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2open/refs/heads/main/openapi/inttra-ocean-execution-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: E2Open Authentication
name_suffix: Authentication
oauth_flows: []
overview: e2open secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: e2open
provider_slug: e2open
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from the INTTRA identity service
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/inttra-ocean-execution-openapi.yml
  type: http
slug: e2open-authentication
source_filename: e2open-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inttra-ocean-execution-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from the INTTRA identity service\n  sources:\n  - openapi/inttra-ocean-execution-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2open/refs/heads/main/authentication/e2open-authentication.yml
summary_line: http · 1 scheme
tags: []
---
