---
api_key_in: []
api_specs:
- filename: sysco-food-distribution-api-openapi.yml
  format: yaml
  label: Sysco Food Distribution API
  slug: food-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysco/refs/heads/main/openapi/sysco-food-distribution-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sysco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sysco secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sysco
provider_slug: sysco
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sysco-food-distribution-api-openapi.yml
  type: http
slug: sysco-authentication
source_filename: sysco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sysco-food-distribution-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sysco-food-distribution-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysco/refs/heads/main/authentication/sysco-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 100
- Food Distribution
- Food Service
- Supply Chain
- Fortune 100
- Wholesale
---
