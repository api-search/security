---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: Coscine Research Data API
  slug: coscine
  spec_type: OpenAPI
  url: https://coscine.rwth-aachen.de/coscine/api/swagger/v2/swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rwth Aachen University Authentication
name_suffix: Authentication
oauth_flows: []
overview: RWTH Aachen University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RWTH Aachen University
provider_slug: rwth-aachen-university
scheme_count: 1
schemes:
- description: JWT Authorization header using the Bearer scheme.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/rwth-aachen-university-coscine.yaml
  type: apiKey
slug: rwth-aachen-university-authentication
source_filename: rwth-aachen-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rwth-aachen-university-coscine.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT Authorization header using the Bearer scheme.\n  sources:\n  - openapi/rwth-aachen-university-coscine.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rwth-aachen-university/refs/heads/main/authentication/rwth-aachen-university-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Germany
---
