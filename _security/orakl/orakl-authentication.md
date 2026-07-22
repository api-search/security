---
api_key_in: []
api_specs:
- filename: orakl-website-openapi-original.json
  format: json
  label: Orakl Oncology Public Website API
  slug: orakl-oncology-public-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-website-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orakl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orakl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orakl
provider_slug: orakl
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: JWT
  scheme: bearer
  sources:
  - openapi/orakl-website-openapi-original.json
  type: http
slug: orakl-authentication
source_filename: orakl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orakl-website-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/orakl-website-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/authentication/orakl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- TechBio
- Oncology
- Drug Development
- Artificial Intelligence
- Machine Learning
- Healthcare
- Biotechnology
- Precision Medicine
- Cancer Research
- Content Management
- JSON-LD
---
