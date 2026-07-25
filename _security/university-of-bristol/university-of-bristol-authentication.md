---
api_key_in:
- header
api_specs:
- filename: university-of-bristol-data-set-api-openapi.yml
  format: yaml
  label: University of Bristol data-set API
  slug: university-of-bristol-data-set-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/openapi/university-of-bristol-data-set-api-openapi.yml
- filename: university-of-bristol-person-api-openapi.yml
  format: yaml
  label: University of Bristol person API
  slug: university-of-bristol-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/openapi/university-of-bristol-person-api-openapi.yml
- filename: university-of-bristol-project-api-openapi.yml
  format: yaml
  label: University of Bristol project API
  slug: university-of-bristol-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/openapi/university-of-bristol-project-api-openapi.yml
- filename: university-of-bristol-research-output-api-openapi.yml
  format: yaml
  label: University of Bristol research-output API
  slug: university-of-bristol-research-output-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/openapi/university-of-bristol-research-output-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Bristol Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Bristol secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Bristol
provider_slug: university-of-bristol
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/university-of-bristol-pure-research-api.yaml
  type: apiKey
slug: university-of-bristol-authentication
source_filename: university-of-bristol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-bristol-pure-research-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/university-of-bristol-pure-research-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/authentication/university-of-bristol-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United Kingdom
---
