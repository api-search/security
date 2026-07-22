---
api_key_in:
- header
- query
api_specs:
- filename: sofar-ocean-spotter-openapi.yml
  format: yaml
  label: Spotter & Smart Mooring API
  slug: spotter-smart-mooring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofar-ocean/refs/heads/main/openapi/sofar-ocean-spotter-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sofar Ocean Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sofar Ocean secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sofar Ocean
provider_slug: sofar-ocean
scheme_count: 2
schemes:
- description: API token tied to your Sofar account, generated at spotter.sofarocean.com/api.
  in: header
  name: tokenHeader
  parameter: token
  sources:
  - openapi/sofar-ocean-spotter-openapi.yml
  type: apiKey
- description: API token passed as a query parameter.
  in: query
  name: tokenQuery
  parameter: token
  sources:
  - openapi/sofar-ocean-spotter-openapi.yml
  type: apiKey
slug: sofar-ocean-authentication
source_filename: sofar-ocean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sofar-ocean-spotter-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: token\n  description: API token tied to your Sofar account, generated at spotter.sofarocean.com/api.\n  sources:\n  - openapi/sofar-ocean-spotter-openapi.yml\n- name: tokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token passed as a query parameter.\n  sources:\n  - openapi/sofar-ocean-spotter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofar-ocean/refs/heads/main/authentication/sofar-ocean-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Climate
- Ocean Data
- Weather
- Maritime
- Sensors
- IoT
- Environmental Data
- Wave Data
- Buoys
---
