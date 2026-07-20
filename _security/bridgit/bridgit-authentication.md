---
api_key_in: []
api_specs:
- filename: index.html
  format: yaml
  label: Bridgit Bench API
  slug: bridgit-bench
  spec_type: OpenAPI
  url: https://bench.gobridgit.com/rp/swagger/index.html
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bridgit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bridgit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bridgit
provider_slug: bridgit
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Standard Authorization header using the Bearer scheme
  name: Bearer
  scheme: bearer
  sources:
  - openapi/bridgit-bench-openapi.yml
  type: http
slug: bridgit-authentication
source_filename: bridgit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bridgit-bench-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Standard Authorization header using the Bearer scheme\n  sources:\n  - openapi/bridgit-bench-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgit/refs/heads/main/authentication/bridgit-authentication.yml
summary_line: http · 1 scheme
tags:
- Construction
- Construction Technology
- Workforce Planning
- Workforce Management
- Resource Planning
- Project Staffing
- General Contractors
- Subcontractors
- Forecasting
- Utilization
- Certifications
- AEC
- SaaS
---
