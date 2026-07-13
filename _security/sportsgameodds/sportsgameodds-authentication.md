---
api_key_in:
- header
api_specs:
- filename: sportsgameodds-openapi.yml
  format: yaml
  label: SportsGameOdds API
  slug: sportsgameodds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportsgameodds Authentication
name_suffix: Authentication
oauth_flows: []
overview: SportsGameOdds secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SportsGameOdds
provider_slug: sportsgameodds
scheme_count: 1
schemes:
- in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/sportsgameodds-openapi.yml
  type: apiKey
slug: sportsgameodds-authentication
source_filename: sportsgameodds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportsgameodds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/sportsgameodds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/authentication/sportsgameodds-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports Betting
- Odds
- Sports Data
- Fantasy Sports
- Gambling
---
