---
api_key_in:
- header
api_specs:
- filename: university-of-manchester-pure-rest.yaml
  format: yaml
  label: Pure CRIS REST API
  slug: pure-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-pure-rest.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Manchester Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Manchester secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Manchester
provider_slug: university-of-manchester
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/university-of-manchester-pure-rest.yaml
  type: apiKey
slug: university-of-manchester-authentication
source_filename: university-of-manchester-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-manchester-pure-rest.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/university-of-manchester-pure-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/authentication/university-of-manchester-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United Kingdom
---
