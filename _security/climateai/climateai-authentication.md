---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Climateai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClimateAI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClimateAI
provider_slug: climateai
scheme_count: 2
schemes:
- in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/climateai-platform-swagger.json
  type: apiKey
- in: header
  name: apikey
  parameter: X-Api-Key
  sources:
  - openapi/climateai-platform-swagger.json
  - openapi/climateai-weather-openapi.yml
  type: apiKey
slug: climateai-authentication
source_filename: climateai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/climateai-platform-swagger.json, openapi/climateai-weather-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/climateai-platform-swagger.json\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/climateai-platform-swagger.json\n  - openapi/climateai-weather-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/authentication/climateai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
---
