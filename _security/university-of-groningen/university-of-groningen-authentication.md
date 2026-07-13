---
api_key_in:
- header
api_specs:
- filename: university-of-groningen-pure-rest-api.yaml
  format: yaml
  label: UG Pure Web Services REST API
  slug: pure-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-pure-rest-api.yaml
- filename: university-of-groningen-dataversenl-native-api.yaml
  format: yaml
  label: DataverseNL Native REST API (UG Default Data Repository)
  slug: dataversenl-native-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-dataversenl-native-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Groningen Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Groningen secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Groningen
provider_slug: university-of-groningen
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/university-of-groningen-pure-rest-api.yaml
  type: apiKey
slug: university-of-groningen-authentication
source_filename: university-of-groningen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-groningen-pure-rest-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/university-of-groningen-pure-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/authentication/university-of-groningen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Research Data
- Library
- Metadata
- Netherlands
- Europe
---
