---
api_key_in:
- header
api_specs:
- filename: aarhus-pure-rest.yaml
  format: yaml
  label: Pure Research Portal Web Service (REST)
  slug: pure-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarhus/refs/heads/main/openapi/aarhus-pure-rest.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aarhus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aarhus University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aarhus University
provider_slug: aarhus
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/aarhus-pure-rest.yaml
  type: apiKey
slug: aarhus-authentication
source_filename: aarhus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aarhus-pure-rest.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/aarhus-pure-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aarhus/refs/heads/main/authentication/aarhus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Denmark
- Europe
---
