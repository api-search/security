---
api_key_in:
- header
- query
api_specs:
- filename: sportsdataio-nfl-openapi.yml
  format: yaml
  label: SportsDataIO NFL API
  slug: sportsdataio-nfl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nfl-openapi.yml
- filename: sportsdataio-mlb-openapi.yml
  format: yaml
  label: SportsDataIO MLB API
  slug: sportsdataio-mlb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-mlb-openapi.yml
- filename: sportsdataio-nba-openapi.yml
  format: yaml
  label: SportsDataIO NBA API
  slug: sportsdataio-nba
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nba-openapi.yml
- filename: sportsdataio-nhl-openapi.yml
  format: yaml
  label: SportsDataIO NHL API
  slug: sportsdataio-nhl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nhl-openapi.yml
- filename: sportsdataio-soccer-openapi.yml
  format: yaml
  label: SportsDataIO Soccer API
  slug: sportsdataio-soccer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-soccer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportsdataio Authentication
name_suffix: Authentication
oauth_flows: []
overview: SportsDataIO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SportsDataIO
provider_slug: sportsdataio
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/sportsdataio-mlb-openapi.yml
  - openapi/sportsdataio-nba-openapi.yml
  - openapi/sportsdataio-nfl-openapi.yml
  - openapi/sportsdataio-nhl-openapi.yml
  - openapi/sportsdataio-soccer-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/sportsdataio-mlb-openapi.yml
  - openapi/sportsdataio-nba-openapi.yml
  - openapi/sportsdataio-nfl-openapi.yml
  - openapi/sportsdataio-nhl-openapi.yml
  - openapi/sportsdataio-soccer-openapi.yml
  type: apiKey
slug: sportsdataio-authentication
source_filename: sportsdataio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportsdataio-mlb-openapi.yml, openapi/sportsdataio-nba-openapi.yml, openapi/sportsdataio-nfl-openapi.yml,\n  openapi/sportsdataio-nhl-openapi.yml, openapi/sportsdataio-soccer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/sportsdataio-mlb-openapi.yml\n  - openapi/sportsdataio-nba-openapi.yml\n  - openapi/sportsdataio-nfl-openapi.yml\n  - openapi/sportsdataio-nhl-openapi.yml\n  - openapi/sportsdataio-soccer-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/sportsdataio-mlb-openapi.yml\n  - openapi/sportsdataio-nba-openapi.yml\n  - openapi/sportsdataio-nfl-openapi.yml\n  - openapi/sportsdataio-nhl-openapi.yml\n  - openapi/sportsdataio-soccer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/authentication/sportsdataio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Sports Data
- Statistics
- Live Scores
- Fantasy Sports
- Odds
- NFL
- NBA
- MLB
- NHL
- Soccer
---
