---
api_key_in:
- query
api_specs:
- filename: statorium-games-api-openapi.yml
  format: yaml
  label: Statorium Games API
  slug: statorium-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-games-api-openapi.yml
- filename: statorium-leagues-api-openapi.yml
  format: yaml
  label: Statorium Leagues API
  slug: statorium-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-leagues-api-openapi.yml
- filename: statorium-matches-api-openapi.yml
  format: yaml
  label: Statorium Matches API
  slug: statorium-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-matches-api-openapi.yml
- filename: statorium-news-api-openapi.yml
  format: yaml
  label: Statorium News API
  slug: statorium-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-news-api-openapi.yml
- filename: statorium-players-api-openapi.yml
  format: yaml
  label: Statorium Players API
  slug: statorium-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-players-api-openapi.yml
- filename: statorium-seasons-api-openapi.yml
  format: yaml
  label: Statorium Seasons API
  slug: statorium-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-seasons-api-openapi.yml
- filename: statorium-standings-api-openapi.yml
  format: yaml
  label: Statorium Standings API
  slug: statorium-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-standings-api-openapi.yml
- filename: statorium-teams-api-openapi.yml
  format: yaml
  label: Statorium Teams API
  slug: statorium-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-teams-api-openapi.yml
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
