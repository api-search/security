---
api_key_in:
- header
- query
api_specs:
- filename: sportmonks-football-openapi.yml
  format: yaml
  label: Sportmonks Football API
  slug: football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-football-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportmonks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sportmonks secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sportmonks
provider_slug: sportmonks
scheme_count: 2
schemes:
- description: Sportmonks API token passed as the value of the Authorization header.
  in: header
  name: ApiTokenHeader
  parameter: Authorization
  sources:
  - openapi/sportmonks-football-openapi.yml
  type: apiKey
- description: Sportmonks API token passed as the api_token query parameter.
  in: query
  name: ApiTokenQuery
  parameter: api_token
  sources:
  - openapi/sportmonks-football-openapi.yml
  type: apiKey
slug: sportmonks-authentication
source_filename: sportmonks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportmonks-football-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiTokenHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Sportmonks API token passed as the value of the Authorization header.\n  sources:\n  - openapi/sportmonks-football-openapi.yml\n- name: ApiTokenQuery\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: Sportmonks API token passed as the api_token query parameter.\n  sources:\n  - openapi/sportmonks-football-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/authentication/sportmonks-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cricket
- Data
- Developer-Friendly
- Football
- Formula 1
- Livescores
- Motorsport
- Real-Time
- Soccer
- Sports
- Sports Data
- Statistics
---
