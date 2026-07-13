---
api_key_in: []
api_specs:
- filename: permit-io-openapi.json
  format: json
  label: Permit.io API
  slug: permit-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permit-io/refs/heads/main/openapi/permit-io-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Permit Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Permit.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Permit.io
provider_slug: permit-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Authorization header, we support the bearer authentication scheme (see: RFC 6750)'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/permit-io-openapi.json
  type: http
slug: permit-io-authentication
source_filename: permit-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/permit-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Authorization header, we support the bearer authentication scheme (see: RFC\n    6750)'\n  sources:\n  - openapi/permit-io-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permit-io/refs/heads/main/authentication/permit-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Control
- Authorization
- Identity
- Policy
- Security
---
