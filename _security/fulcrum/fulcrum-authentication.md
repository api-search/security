---
api_key_in:
- header
api_specs:
- filename: fulcrum-api-openapi.yml
  format: yaml
  label: Fulcrum API
  slug: fulcrum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fulcrum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fulcrum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fulcrum
provider_slug: fulcrum
scheme_count: 1
schemes:
- description: Fulcrum API token issued from a Fulcrum account
  in: header
  name: ApiToken
  parameter: X-ApiToken
  sources:
  - openapi/fulcrum-api-openapi.yml
  type: apiKey
slug: fulcrum-authentication
source_filename: fulcrum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fulcrum-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-ApiToken\n  description: Fulcrum API token issued from a Fulcrum account\n  sources:\n  - openapi/fulcrum-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/authentication/fulcrum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Collection
- Field Data
- Geospatial
- Process Management
- Mobile
---
