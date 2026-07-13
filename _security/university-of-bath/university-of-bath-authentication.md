---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Bath Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Bath secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Bath
provider_slug: university-of-bath
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/university-of-bath-pure-api.yaml
  type: apiKey
slug: university-of-bath-authentication
source_filename: university-of-bath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-bath-pure-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/university-of-bath-pure-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bath/refs/heads/main/authentication/university-of-bath-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research
- Open Data
- Library
- Metadata
---
