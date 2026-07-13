---
api_key_in:
- query
api_specs:
- filename: cornell-codi-classes.yaml
  format: yaml
  label: Cornell Open Data Initiative (CODI)
  slug: codi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-codi-classes.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cornell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cornell University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cornell University
provider_slug: cornell
scheme_count: 1
schemes:
- description: Security for the API key
  in: query
  name: UserSecurity
  parameter: api_key
  sources:
  - openapi/cornell-codi-events.yaml
  type: apiKey
slug: cornell-authentication
source_filename: cornell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cornell-codi-events.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: UserSecurity\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Security for the API key\n  sources:\n  - openapi/cornell-codi-events.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/authentication/cornell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Course Catalog
- Library
- Research
- United States
---
