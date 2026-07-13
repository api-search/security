---
api_key_in: []
api_specs:
- filename: university-of-amsterdam-lod-triply-api.yaml
  format: yaml
  label: UvA Library Linked Open Data API (Triply)
  slug: lod-triply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-lod-triply-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Amsterdam Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Amsterdam secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Amsterdam
provider_slug: university-of-amsterdam
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/university-of-amsterdam-lod-triply-api.yaml
  type: http
slug: university-of-amsterdam-authentication
source_filename: university-of-amsterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-amsterdam-lod-triply-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/university-of-amsterdam-lod-triply-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/authentication/university-of-amsterdam-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Linked Data
- Library
- Netherlands
- Europe
---
