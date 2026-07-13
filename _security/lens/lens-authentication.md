---
api_key_in: []
api_specs:
- filename: lens-openapi.yml
  format: yaml
  label: Lens API
  slug: lens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lens/refs/heads/main/openapi/lens-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lens secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lens
provider_slug: lens
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API token issued from the Lens user profile (Plans & Tokens).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lens-openapi.yml
  type: http
slug: lens-authentication
source_filename: lens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lens-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API token issued from the Lens user profile (Plans & Tokens).\n  sources:\n  - openapi/lens-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lens/refs/heads/main/authentication/lens-authentication.yml
summary_line: http · 1 scheme
tags:
- Scholarly
- Patents
- Research
- Science
- Open Data
---
