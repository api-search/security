---
api_key_in: []
api_specs:
- filename: tropic-openapi.yml
  format: yaml
  label: Tropic API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tropic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tropic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tropic
provider_slug: tropic
scheme_count: 1
schemes:
- description: API key issued from the Tropic settings panel
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tropic-openapi.yml
  type: http
slug: tropic-authentication
source_filename: tropic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tropic-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued from the Tropic settings panel\n  sources:\n  - openapi/tropic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/authentication/tropic-authentication.yml
summary_line: http · 1 scheme
tags:
- Benchmarking
- Contract Management
- Cost Optimization
- Procurement
- Renewals
- SaaS Management
- SaaS Procurement
- Spend Management
- Supplier Management
---
