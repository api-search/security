---
api_key_in:
- header
api_specs:
- filename: recreation-gov-openapi.yml
  format: yaml
  label: Recreation.gov RIDB API
  slug: ridb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Recreation Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recreation.gov secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recreation.gov
provider_slug: recreation-gov
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/recreation-gov-openapi.yml
  type: apiKey
slug: recreation-gov-authentication
source_filename: recreation-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/recreation-gov-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/recreation-gov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/authentication/recreation-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Recreation
- Federal
- Camping
- Outdoors
- Public Lands
---
