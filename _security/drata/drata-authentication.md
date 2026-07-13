---
api_key_in: []
api_specs:
- filename: drata-openapi.yml
  format: yaml
  label: Drata Public API v2
  slug: public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drata
provider_slug: drata
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drata-openapi.yml
  type: http
slug: drata-authentication
source_filename: drata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/drata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/authentication/drata-authentication.yml
summary_line: http · 1 scheme
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---
