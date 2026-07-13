---
api_key_in:
- header
api_specs:
- filename: vrije-universiteit-amsterdam-pure-web-service.yaml
  format: yaml
  label: VU Research Portal Pure Web Service (REST)
  slug: pure-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vrije-universiteit-amsterdam/refs/heads/main/openapi/vrije-universiteit-amsterdam-pure-web-service.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vrije Universiteit Amsterdam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vrije Universiteit Amsterdam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vrije Universiteit Amsterdam
provider_slug: vrije-universiteit-amsterdam
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/vrije-universiteit-amsterdam-pure-web-service.yaml
  type: apiKey
slug: vrije-universiteit-amsterdam-authentication
source_filename: vrije-universiteit-amsterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vrije-universiteit-amsterdam-pure-web-service.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/vrije-universiteit-amsterdam-pure-web-service.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrije-universiteit-amsterdam/refs/heads/main/authentication/vrije-universiteit-amsterdam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Netherlands
- Research
- Open Data
- Repository
---
