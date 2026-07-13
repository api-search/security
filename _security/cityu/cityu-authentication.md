---
api_key_in:
- header
api_specs:
- filename: cityu-scholars-pure-ws.yaml
  format: yaml
  label: CityUHK Scholars Pure Web Service (REST)
  slug: scholars-pure-ws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/openapi/cityu-scholars-pure-ws.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cityu Authentication
name_suffix: Authentication
oauth_flows: []
overview: City University of Hong Kong secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: City University of Hong Kong
provider_slug: cityu
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/cityu-scholars-pure-ws.yaml
  type: apiKey
slug: cityu-authentication
source_filename: cityu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cityu-scholars-pure-ws.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/cityu-scholars-pure-ws.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/authentication/cityu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- OAI-PMH
- Hong Kong
- China
---
