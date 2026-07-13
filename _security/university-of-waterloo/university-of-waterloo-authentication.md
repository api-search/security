---
api_key_in:
- header
api_specs:
- filename: university-of-waterloo-open-data-api.yaml
  format: yaml
  label: University of Waterloo Open Data API (v3)
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-open-data-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Waterloo Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Waterloo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Waterloo
provider_slug: university-of-waterloo
scheme_count: 1
schemes:
- description: Custom API key authentication
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/university-of-waterloo-open-data-api.yaml
  type: apiKey
slug: university-of-waterloo-authentication
source_filename: university-of-waterloo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-waterloo-open-data-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Custom API key authentication\n  sources:\n  - openapi/university-of-waterloo-open-data-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/authentication/university-of-waterloo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Canada
- Research
---
