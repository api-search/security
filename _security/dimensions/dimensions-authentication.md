---
api_key_in:
- header
api_specs:
- filename: dimensions-openapi.yml
  format: yaml
  label: Dimensions Analytics API
  slug: dimensions-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dimensions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dimensions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dimensions
provider_slug: dimensions
scheme_count: 1
schemes:
- description: Pass `JWT {token}` returned by /auth
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/dimensions-openapi.yml
  type: apiKey
slug: dimensions-authentication
source_filename: dimensions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dimensions-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Pass `JWT {token}` returned by /auth\n  sources:\n  - openapi/dimensions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/authentication/dimensions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Research
- Publications
- Grants
- Patents
- Clinical Trials
- Jupyter Notebooks
---
