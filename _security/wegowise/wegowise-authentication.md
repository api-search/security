---
api_key_in: []
api_specs:
- filename: wegowise-openapi.yml
  format: yaml
  label: WegoWise API
  slug: wegowise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wegowise Authentication
name_suffix: Authentication
oauth_flows: []
overview: WegoWise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WegoWise
provider_slug: wegowise
scheme_count: 1
schemes:
- description: OAuth 1.0 authentication required for private endpoints
  name: oauth1
  scheme: oauth
  sources:
  - openapi/wegowise-openapi.yml
  type: http
slug: wegowise-authentication
source_filename: wegowise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wegowise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth1\n  type: http\n  scheme: oauth\n  description: OAuth 1.0 authentication required for private endpoints\n  sources:\n  - openapi/wegowise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/authentication/wegowise-authentication.yml
summary_line: http · 1 scheme
tags:
- Benchmarking
- Building Energy
- Energy Efficiency
- Multifamily
- Property Management
- Utility Data
---
