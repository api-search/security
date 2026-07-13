---
api_key_in:
- header
api_specs:
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Sports Odds
  slug: wager-api-odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Fantasy Sports Data
  slug: wager-api-fantasy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wager Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wager API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wager API
provider_slug: wager-api
scheme_count: 1
schemes:
- description: API key obtained from Wager API, request via wagerapi.com
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/wager-api-openapi.yml
  type: apiKey
slug: wager-api-authentication
source_filename: wager-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wager-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key obtained from Wager API, request via wagerapi.com\n  sources:\n  - openapi/wager-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/authentication/wager-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports Betting
- Sports Odds
- Fantasy Sports
- Sports Data
- NFL
- NBA
- MLB
- NHL
- NCAA
---
