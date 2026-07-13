---
api_key_in:
- header
api_specs:
- filename: sportsbook-api-openapi.yml
  format: yaml
  label: Sportsbook API
  slug: sportsbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsbook-api/refs/heads/main/openapi/sportsbook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportsbook Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sportsbook API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sportsbook API
provider_slug: sportsbook-api
scheme_count: 1
schemes:
- in: header
  name: rapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/sportsbook-api-openapi.yml
  type: apiKey
slug: sportsbook-api-authentication
source_filename: sportsbook-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportsbook-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  sources:\n  - openapi/sportsbook-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsbook-api/refs/heads/main/authentication/sportsbook-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports Betting
- Odds
- Sports Data
- Gambling
---
