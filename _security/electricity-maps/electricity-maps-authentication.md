---
api_key_in:
- header
api_specs:
- filename: electricity-maps-openapi.yml
  format: yaml
  label: Electricity Maps API
  slug: electricity-maps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-maps/refs/heads/main/openapi/electricity-maps-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Electricity Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electricity Maps secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Electricity Maps
provider_slug: electricity-maps
scheme_count: 2
schemes:
- description: API token issued from the Electricity Maps portal.
  in: header
  name: authToken
  parameter: auth-token
  sources:
  - openapi/electricity-maps-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/electricity-maps-openapi.yml
  type: http
slug: electricity-maps-authentication
source_filename: electricity-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/electricity-maps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: auth-token\n  description: API token issued from the Electricity Maps portal.\n  sources:\n  - openapi/electricity-maps-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/electricity-maps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricity-maps/refs/heads/main/authentication/electricity-maps-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Energy
- Electricity
- Carbon Intensity
- Sustainability
- Climate
- Grid Data
---
