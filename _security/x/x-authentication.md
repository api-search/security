---
api_key_in: []
api_specs:
- filename: x-openapi.yml
  format: yaml
  label: X
  slug: x
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: X Authentication
name_suffix: Authentication
oauth_flows: []
overview: X secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: X
provider_slug: x
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'App-only authentication using an OAuth 2.0 Bearer Token issued by the

    X Developer Platform, passed via the Authorization header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/x-openapi.yml
  type: http
slug: x-authentication
source_filename: x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/x-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    App-only authentication using an OAuth 2.0 Bearer Token issued by the\n    X Developer Platform, passed via the Authorization header.\n  sources:\n  - openapi/x-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/authentication/x-authentication.yml
summary_line: http · 1 scheme
tags: []
---
