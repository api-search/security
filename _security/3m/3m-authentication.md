---
api_key_in: []
api_specs:
- filename: 3m-partner-supplier-api-openapi.yml
  format: yaml
  label: 3M Partner and Supplier API
  slug: partner-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/openapi/3m-partner-supplier-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 3M Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3M secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 3M
provider_slug: 3m
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained through client credentials flow. Provided during onboarding.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/3m-partner-supplier-api-openapi.yml
  type: http
slug: 3m-authentication
source_filename: 3m-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/3m-partner-supplier-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained through client credentials flow. Provided during\n    onboarding.\n  sources:\n  - openapi/3m-partner-supplier-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/authentication/3m-authentication.yml
summary_line: http · 1 scheme
tags:
- Industrial
- Manufacturing
- Supply Chain
- Fortune 100
---
