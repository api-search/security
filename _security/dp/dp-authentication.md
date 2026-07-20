---
api_key_in: []
api_specs:
- filename: dp-bohrium-openapi.json
  format: json
  label: Bohrium OpenAPI
  slug: bohrium-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dp Authentication
name_suffix: Authentication
oauth_flows: []
overview: DP Technology (Bohrium) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DP Technology (Bohrium)
provider_slug: dp
scheme_count: 1
schemes:
- description: Bohrium AccessKey，环境变量 BOHR_ACCESS_KEY，作为 Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dp-bohrium-openapi.json
  type: http
slug: dp-authentication
source_filename: dp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dp-bohrium-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bohrium AccessKey，环境变量 BOHR_ACCESS_KEY，作为 Bearer token\n  sources:\n  - openapi/dp-bohrium-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/authentication/dp-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI for Science
- Scientific Computing
- Molecular Simulation
- Drug Discovery
- Materials Science
- Research Cloud
- Machine Learning
- HPC
---
