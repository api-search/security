---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Gett Business API
  slug: gett-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gett Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gett secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gett
provider_slug: gett
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from /oauth/token endpoint. Valid for 899 seconds.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: gett-authentication
source_filename: gett-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from /oauth/token endpoint. Valid for 899 seconds.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/authentication/gett-authentication.yml
summary_line: http · 1 scheme
tags:
- Ground Transportation
- Corporate Travel
- Ride Booking
- Business Travel
- Expense Management
---
