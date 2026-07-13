---
api_key_in: []
api_specs:
- filename: basiq-api-openapi.yml
  format: yaml
  label: Basiq API
  slug: basiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Basiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basiq
provider_slug: basiq
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/basiq-api-openapi.yml
  type: http
slug: basiq-authentication
source_filename: basiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basiq-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/basiq-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/authentication/basiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
---
