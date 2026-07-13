---
api_key_in:
- query
api_specs:
- filename: revolutio-hazard-api-openapi.yml
  format: yaml
  label: Revolutio Hazard API
  slug: revolutio-hazard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/openapi/revolutio-hazard-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revolutio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revolutio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revolutio
provider_slug: revolutio
scheme_count: 1
schemes:
- description: Revolutio Hazard API subscription key. For POST requests pass in request header.
  in: query
  name: HazardApiKey
  parameter: apiKey
  sources:
  - openapi/revolutio-hazard-api-openapi.yml
  type: apiKey
slug: revolutio-authentication
source_filename: revolutio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revolutio-hazard-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: HazardApiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Revolutio Hazard API subscription key. For POST requests pass in request header.\n  sources:\n  - openapi/revolutio-hazard-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/authentication/revolutio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Engineering
- Hazard
- Weather
- Structural Engineering
- Wind Analysis
- Construction
---
