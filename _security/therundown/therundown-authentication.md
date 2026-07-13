---
api_key_in:
- header
- query
api_specs:
- filename: list-all-sports
  format: yaml
  label: TheRundown Sports Odds API
  slug: sports-odds-api
  spec_type: OpenAPI
  url: https://docs.therundown.io/api-reference/generated/v2-sports/list-all-sports
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Therundown Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Rundown secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: The Rundown
provider_slug: therundown
scheme_count: 2
schemes:
- description: API key as query parameter
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/therundown-sports-odds-api-openapi.yml
  type: apiKey
- description: API key as request header
  in: header
  name: ApiKeyHeader
  parameter: X-Therundown-Key
  sources:
  - openapi/therundown-sports-odds-api-openapi.yml
  type: apiKey
slug: therundown-authentication
source_filename: therundown-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/therundown-sports-odds-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key as query parameter\n  sources:\n  - openapi/therundown-sports-odds-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Therundown-Key\n  description: API key as request header\n  sources:\n  - openapi/therundown-sports-odds-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/authentication/therundown-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Sports
- Betting
- Odds
- NFL
- NBA
- MLB
- NHL
- Soccer
- Real-Time
- Sports Data
- Sportsbook
---
