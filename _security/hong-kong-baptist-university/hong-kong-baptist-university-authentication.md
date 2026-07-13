---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: HKBU Scholars Pure Web Service API
  slug: pure-research-api
  spec_type: OpenAPI
  url: https://scholars.hkbu.edu.hk/ws/api/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hong Kong Baptist University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hong Kong Baptist University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hong Kong Baptist University
provider_slug: hong-kong-baptist-university
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/hong-kong-baptist-university-pure-research-api.yaml
  type: apiKey
slug: hong-kong-baptist-university-authentication
source_filename: hong-kong-baptist-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hong-kong-baptist-university-pure-research-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/hong-kong-baptist-university-pure-research-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/authentication/hong-kong-baptist-university-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Hong Kong
- Pure
- Research Information
---
