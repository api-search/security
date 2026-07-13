---
api_key_in:
- header
api_specs:
- filename: queens-university-belfast-pure-api.yaml
  format: yaml
  label: Queen's University Belfast Research Portal (Pure REST API)
  slug: pure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/queens-university-belfast/refs/heads/main/openapi/queens-university-belfast-pure-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Queens University Belfast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Queen's University Belfast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Queen's University Belfast
provider_slug: queens-university-belfast
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/queens-university-belfast-pure-api.yaml
  type: apiKey
slug: queens-university-belfast-authentication
source_filename: queens-university-belfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/queens-university-belfast-pure-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/queens-university-belfast-pure-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queens-university-belfast/refs/heads/main/authentication/queens-university-belfast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- OAI-PMH
- United Kingdom
- Northern Ireland
---
