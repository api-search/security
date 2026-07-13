---
api_key_in:
- header
api_specs:
- filename: blablacar-bus-api-openapi.yaml
  format: yaml
  label: BlaBlaCar Bus API
  slug: blablacar-bus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blablacar Bus Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlaBlaCar Bus API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
scheme_count: 1
schemes:
- description: API key provided by BlaBlaCar Bus partner program
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/blablacar-bus-api-openapi.yaml
  type: apiKey
slug: blablacar-bus-api-authentication
source_filename: blablacar-bus-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blablacar-bus-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key provided by BlaBlaCar Bus partner program\n  sources:\n  - openapi/blablacar-bus-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/authentication/blablacar-bus-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
---
