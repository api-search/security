---
api_key_in:
- header
api_specs:
- filename: rentcast-openapi.json
  format: json
  label: RentCast API
  slug: rentcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/openapi/rentcast-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rentcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: RentCast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RentCast
provider_slug: rentcast
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: X-Api-Key
  sources:
  - openapi/rentcast-openapi.json
  type: apiKey
slug: rentcast-authentication
source_filename: rentcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rentcast-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/rentcast-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/authentication/rentcast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- Property Data
- Valuation
- Rental Market
- AVM
---
