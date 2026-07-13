---
api_key_in:
- header
api_specs:
- filename: eindhoven-university-of-technology-pure-web-service.yaml
  format: yaml
  label: TU/e Pure Web Service (Research API)
  slug: pure-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eindhoven-university-of-technology/refs/heads/main/openapi/eindhoven-university-of-technology-pure-web-service.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eindhoven University Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eindhoven University of Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eindhoven University of Technology
provider_slug: eindhoven-university-of-technology
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/eindhoven-university-of-technology-pure-web-service.yaml
  type: apiKey
slug: eindhoven-university-of-technology-authentication
source_filename: eindhoven-university-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eindhoven-university-of-technology-pure-web-service.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/eindhoven-university-of-technology-pure-web-service.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eindhoven-university-of-technology/refs/heads/main/authentication/eindhoven-university-of-technology-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Netherlands
- Europe
---
