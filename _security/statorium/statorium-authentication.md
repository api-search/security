---
api_key_in:
- query
api_specs:
- filename: statorium-football-api-openapi.yml
  format: yaml
  label: Statorium Football API
  slug: football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-football-api-openapi.yml
- filename: statorium-basketball-api-openapi.yml
  format: yaml
  label: Statorium Basketball API
  slug: basketball-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-basketball-api-openapi.yml
- filename: statorium-american-football-api-openapi.yml
  format: yaml
  label: Statorium American Football API
  slug: american-football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-american-football-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Statorium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Statorium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Statorium
provider_slug: statorium
scheme_count: 1
schemes:
- description: API token provided upon subscription purchase.
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/statorium-american-football-api-openapi.yml
  - openapi/statorium-basketball-api-openapi.yml
  - openapi/statorium-football-api-openapi.yml
  type: apiKey
slug: statorium-authentication
source_filename: statorium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/statorium-american-football-api-openapi.yml, openapi/statorium-basketball-api-openapi.yml,\n  openapi/statorium-football-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API token provided upon subscription purchase.\n  sources:\n  - openapi/statorium-american-football-api-openapi.yml\n  - openapi/statorium-basketball-api-openapi.yml\n  - openapi/statorium-football-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/authentication/statorium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Sports Data
- Football
- Soccer
- Basketball
- American Football
- Live Scores
- Statistics
---
