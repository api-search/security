---
api_key_in:
- header
api_specs:
- filename: uppsala-ucdp.yaml
  format: yaml
  label: UCDP API
  slug: ucdp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-ucdp.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uppsala Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uppsala University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uppsala University
provider_slug: uppsala
scheme_count: 1
schemes:
- description: UCDP API token sent in x-ucdp-access-token header
  in: header
  name: ApiToken
  parameter: x-ucdp-access-token
  sources:
  - openapi/uppsala-ucdp.yaml
  type: apiKey
slug: uppsala-authentication
source_filename: uppsala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uppsala-ucdp.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: x-ucdp-access-token\n  description: UCDP API token sent in x-ucdp-access-token header\n  sources:\n  - openapi/uppsala-ucdp.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/authentication/uppsala-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Sweden
---
