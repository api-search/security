---
api_key_in: []
api_specs:
- filename: shareworks-shareworks-public-api-openapi.yml
  format: yaml
  label: Shareworks Public API
  slug: shareworks-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-shareworks-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shareworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shareworks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shareworks
provider_slug: shareworks
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: accessToken
  scheme: bearer
  sources:
  - openapi/shareworks-shareworks-public-api-openapi.yml
  type: http
slug: shareworks-authentication
source_filename: shareworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shareworks-shareworks-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/shareworks-shareworks-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/authentication/shareworks-authentication.yml
summary_line: http · 1 scheme
tags:
- Equity Compensation
- Stock Options
- RSU
- ESPP
- Employee Equity
- Financial Services
- Morgan Stanley
- Equity Administration
- Private Companies
- Public Companies
---
