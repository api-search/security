---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 5dollarfootballapi-bookmakers-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Bookmakers API
  slug: 5dollarfootballapi-bookmakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-bookmakers-api-openapi.yml
- filename: 5dollarfootballapi-countries-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Countries API
  slug: 5dollarfootballapi-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-countries-api-openapi.yml
- filename: 5dollarfootballapi-fixtures-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Fixtures API
  slug: 5dollarfootballapi-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-fixtures-api-openapi.yml
- filename: 5dollarfootballapi-leagues-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Leagues API
  slug: 5dollarfootballapi-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-leagues-api-openapi.yml
- filename: 5dollarfootballapi-standings-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Standings API
  slug: 5dollarfootballapi-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-standings-api-openapi.yml
- filename: 5dollarfootballapi-status-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Status API
  slug: 5dollarfootballapi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-status-api-openapi.yml
- filename: 5dollarfootballapi-teams-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Teams API
  slug: 5dollarfootballapi-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-teams-api-openapi.yml
- filename: 5dollarfootballapi-bookmakers-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Bookmakers API
  slug: 5dollarfootballapi-bookmakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-bookmakers-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: 5Dollarfootballapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: 5DollarFootballAPI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 5DollarFootballAPI
provider_slug: 5dollarfootballapi
scheme_count: 2
schemes:
- description: 'Send your key as `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/5dollarfootballapi-bookmakers-api-openapi.yml
  - openapi/5dollarfootballapi-countries-api-openapi.yml
  - openapi/5dollarfootballapi-fixtures-api-openapi.yml
  - openapi/5dollarfootballapi-leagues-api-openapi.yml
  - openapi/5dollarfootballapi-standings-api-openapi.yml
  - openapi/5dollarfootballapi-status-api-openapi.yml
  - openapi/5dollarfootballapi-teams-api-openapi.yml
  type: http
- description: Alternative to the Authorization header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/5dollarfootballapi-bookmakers-api-openapi.yml
  - openapi/5dollarfootballapi-countries-api-openapi.yml
  - openapi/5dollarfootballapi-fixtures-api-openapi.yml
  - openapi/5dollarfootballapi-leagues-api-openapi.yml
  - openapi/5dollarfootballapi-standings-api-openapi.yml
  - openapi/5dollarfootballapi-status-api-openapi.yml
  - openapi/5dollarfootballapi-teams-api-openapi.yml
  type: apiKey
slug: 5dollarfootballapi-authentication
source_filename: 5dollarfootballapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: derived\nsource: openapi/5dollarfootballapi-bookmakers-api-openapi.yml, openapi/5dollarfootballapi-countries-api-openapi.yml,\n  openapi/5dollarfootballapi-fixtures-api-openapi.yml, openapi/5dollarfootballapi-leagues-api-openapi.yml,\n  openapi/5dollarfootballapi-standings-api-openapi.yml, openapi/5dollarfootballapi-status-api-openapi.yml,\n  openapi/5dollarfootballapi-teams-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send your key as `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/5dollarfootballapi-bookmakers-api-openapi.yml\n  - openapi/5dollarfootballapi-countries-api-openapi.yml\n  - openapi/5dollarfootballapi-fixtures-api-openapi.yml\n  - openapi/5dollarfootballapi-leagues-api-openapi.yml\n  - openapi/5dollarfootballapi-standings-api-openapi.yml\n  - openapi/5dollarfootballapi-status-api-openapi.yml\n  - openapi/5dollarfootballapi-teams-api-openapi.yml\n\
  - name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative to the Authorization header.\n  sources:\n  - openapi/5dollarfootballapi-bookmakers-api-openapi.yml\n  - openapi/5dollarfootballapi-countries-api-openapi.yml\n  - openapi/5dollarfootballapi-fixtures-api-openapi.yml\n  - openapi/5dollarfootballapi-leagues-api-openapi.yml\n  - openapi/5dollarfootballapi-standings-api-openapi.yml\n  - openapi/5dollarfootballapi-status-api-openapi.yml\n  - openapi/5dollarfootballapi-teams-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/authentication/5dollarfootballapi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Football
- Soccer
- Sports
- Sports Data
- Live Scores
- Fixtures
- Standings
- Statistics
- Odds
- Bookmakers
---
