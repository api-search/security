---
api_key_in:
- header
- query
api_specs:
- filename: oddsjam-fixtures-api-openapi.yml
  format: yaml
  label: OddsJam Fixtures API
  slug: oddsjam-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-fixtures-api-openapi.yml
- filename: oddsjam-futures-api-openapi.yml
  format: yaml
  label: OddsJam Futures API
  slug: oddsjam-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-futures-api-openapi.yml
- filename: oddsjam-grader-api-openapi.yml
  format: yaml
  label: OddsJam Grader API
  slug: oddsjam-grader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-grader-api-openapi.yml
- filename: oddsjam-injuries-api-openapi.yml
  format: yaml
  label: OddsJam Injuries API
  slug: oddsjam-injuries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-injuries-api-openapi.yml
- filename: oddsjam-leagues-api-openapi.yml
  format: yaml
  label: OddsJam Leagues API
  slug: oddsjam-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-leagues-api-openapi.yml
- filename: oddsjam-markets-api-openapi.yml
  format: yaml
  label: OddsJam Markets API
  slug: oddsjam-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-markets-api-openapi.yml
- filename: oddsjam-players-api-openapi.yml
  format: yaml
  label: OddsJam Players API
  slug: oddsjam-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-players-api-openapi.yml
- filename: oddsjam-sports-api-openapi.yml
  format: yaml
  label: OddsJam Sports API
  slug: oddsjam-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-sports-api-openapi.yml
- filename: oddsjam-sportsbooks-api-openapi.yml
  format: yaml
  label: OddsJam Sportsbooks API
  slug: oddsjam-sportsbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-sportsbooks-api-openapi.yml
- filename: oddsjam-streaming-api-openapi.yml
  format: yaml
  label: OddsJam Streaming API
  slug: oddsjam-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-streaming-api-openapi.yml
- filename: oddsjam-teams-api-openapi.yml
  format: yaml
  label: OddsJam Teams API
  slug: oddsjam-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-teams-api-openapi.yml
- filename: oddsjam-tournaments-api-openapi.yml
  format: yaml
  label: OddsJam Tournaments API
  slug: oddsjam-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-tournaments-api-openapi.yml
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
