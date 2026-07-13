---
api_key_in: []
api_specs:
- filename: perfectscale-perfectscale-openapi.yml
  format: yaml
  label: PerfectScale Public API
  slug: perfectscale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perfectscale/refs/heads/main/openapi/perfectscale-perfectscale-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Perfectscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: PerfectScale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PerfectScale
provider_slug: perfectscale
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/perfectscale-perfectscale-openapi.yml
  type: http
slug: perfectscale-authentication
source_filename: perfectscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/perfectscale-perfectscale-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/perfectscale-perfectscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfectscale/refs/heads/main/authentication/perfectscale-authentication.yml
summary_line: http · 1 scheme
tags:
- FinOps
- Kubernetes
- Cost Optimization
---
