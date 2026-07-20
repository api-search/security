---
api_key_in: []
api_specs:
- filename: biolevate-api-original.json
  format: json
  label: Biolevate API
  slug: biolevate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-api-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Biolevate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biolevate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Biolevate
provider_slug: biolevate
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: TOKEN
  scheme: bearer
  sources:
  - openapi/biolevate-api-original.json
  type: http
slug: biolevate-authentication
source_filename: biolevate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/biolevate-api-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: TOKEN\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/biolevate-api-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/authentication/biolevate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Life Sciences
- Regulatory Affairs
- Document Intelligence
- Knowledge Management
- Pharmaceuticals
- Machine Learning
---
