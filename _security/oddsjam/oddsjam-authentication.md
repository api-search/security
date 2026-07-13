---
api_key_in:
- header
- query
api_specs:
- filename: oddsjam-openapi.yml
  format: yaml
  label: OddsJam API
  slug: oddsjam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oddsjam Authentication
name_suffix: Authentication
oauth_flows: []
overview: OddsJam secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OddsJam
provider_slug: oddsjam
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/oddsjam-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/oddsjam-openapi.yml
  type: apiKey
slug: oddsjam-authentication
source_filename: oddsjam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oddsjam-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/oddsjam-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/oddsjam-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/authentication/oddsjam-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Odds
- Sports Betting
- Sportsbooks
---
