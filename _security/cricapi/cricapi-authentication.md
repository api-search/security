---
api_key_in:
- query
api_specs:
- filename: cricapi-cricket-data-api-openapi.yml
  format: yaml
  label: Cricket Data API
  slug: cricket-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cricapi/refs/heads/main/openapi/cricapi-cricket-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cricapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CricAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CricAPI
provider_slug: cricapi
scheme_count: 1
schemes:
- description: 'API key for authentication. Obtained from your CricketData.org account. Format: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx (GUID)'
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/cricapi-cricket-data-api-openapi.yml
  type: apiKey
slug: cricapi-authentication
source_filename: cricapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cricapi-cricket-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: 'API key for authentication. Obtained from your CricketData.org account. Format:\n    xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx (GUID)'\n  sources:\n  - openapi/cricapi-cricket-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cricapi/refs/heads/main/authentication/cricapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cricket
- Sports
- Live Scores
- Player Statistics
- Match Data
- Fantasy Cricket
- Ball-by-Ball
- Team Rankings
- Schedules
- Sports Data
---
