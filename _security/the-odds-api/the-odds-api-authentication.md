---
api_key_in:
- query
api_specs:
- filename: the-odds-api-events-api-openapi.yml
  format: yaml
  label: The Odds API Events API
  slug: the-odds-api-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-events-api-openapi.yml
- filename: the-odds-api-historical-api-openapi.yml
  format: yaml
  label: The Odds API Historical API
  slug: the-odds-api-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-historical-api-openapi.yml
- filename: the-odds-api-odds-api-openapi.yml
  format: yaml
  label: The Odds API Odds API
  slug: the-odds-api-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-odds-api-openapi.yml
- filename: the-odds-api-participants-api-openapi.yml
  format: yaml
  label: The Odds API Participants API
  slug: the-odds-api-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-participants-api-openapi.yml
- filename: the-odds-api-scores-api-openapi.yml
  format: yaml
  label: The Odds API Scores API
  slug: the-odds-api-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-scores-api-openapi.yml
- filename: the-odds-api-sports-api-openapi.yml
  format: yaml
  label: The Odds API Sports API
  slug: the-odds-api-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/openapi/the-odds-api-sports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Odds Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Odds API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Odds API
provider_slug: the-odds-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/the-odds-api-openapi.yml
  type: apiKey
slug: the-odds-api-authentication
source_filename: the-odds-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-odds-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/the-odds-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-odds-api/refs/heads/main/authentication/the-odds-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Betting
- Odds
- Sports
- Scores
- Historical Data
---
