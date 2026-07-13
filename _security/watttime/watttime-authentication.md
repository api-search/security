---
api_key_in: []
api_specs:
- filename: watttime-openapi.yml
  format: yaml
  label: WattTime API
  slug: watttime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watttime/refs/heads/main/openapi/watttime-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Watttime Authentication
name_suffix: Authentication
oauth_flows: []
overview: WattTime secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WattTime
provider_slug: watttime
scheme_count: 2
schemes:
- description: HTTP Basic Authentication used only for the /login endpoint. Provide username and password to obtain a bearer token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/watttime-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'JWT bearer token obtained from the /login endpoint. Token expires after 30 minutes. Include as Authorization: Bearer {token} header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/watttime-openapi.yml
  type: http
slug: watttime-authentication
source_filename: watttime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/watttime-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication used only for the /login endpoint. Provide username\n    and password to obtain a bearer token.\n  sources:\n  - openapi/watttime-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT bearer token obtained from the /login endpoint. Token expires after 30 minutes.\n    Include as Authorization: Bearer {token} header.'\n  sources:\n  - openapi/watttime-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watttime/refs/heads/main/authentication/watttime-authentication.yml
summary_line: http · 2 schemes
tags:
- Emissions
- Climate
- Carbon
- Energy
- Electricity Grid
- Sustainability
- Clean Energy
---
