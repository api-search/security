---
api_key_in:
- query
api_specs:
- filename: n2yo-openapi.yml
  format: yaml
  label: N2YO.com API
  slug: n2yo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n2yo/main/openapi/n2yo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: N2Yo Authentication
name_suffix: Authentication
oauth_flows: []
overview: N2YO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: N2YO
provider_slug: n2yo
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/n2yo-openapi.yml
  type: apiKey
slug: n2yo-authentication
source_filename: n2yo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/n2yo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/n2yo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n2yo/refs/heads/main/authentication/n2yo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Satellites
- Space
- Tracking
---
