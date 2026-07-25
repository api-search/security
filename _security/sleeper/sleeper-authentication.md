---
api_key_in: []
api_specs:
- filename: sleeper-drafts-api-openapi.yml
  format: yaml
  label: Sleeper Drafts API
  slug: sleeper-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-drafts-api-openapi.yml
- filename: sleeper-leagues-api-openapi.yml
  format: yaml
  label: Sleeper Leagues API
  slug: sleeper-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-leagues-api-openapi.yml
- filename: sleeper-matchups-api-openapi.yml
  format: yaml
  label: Sleeper Matchups API
  slug: sleeper-matchups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-matchups-api-openapi.yml
- filename: sleeper-players-api-openapi.yml
  format: yaml
  label: Sleeper Players API
  slug: sleeper-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-players-api-openapi.yml
- filename: sleeper-playoffs-api-openapi.yml
  format: yaml
  label: Sleeper Playoffs API
  slug: sleeper-playoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-playoffs-api-openapi.yml
- filename: sleeper-state-api-openapi.yml
  format: yaml
  label: Sleeper State API
  slug: sleeper-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-state-api-openapi.yml
- filename: sleeper-transactions-api-openapi.yml
  format: yaml
  label: Sleeper Transactions API
  slug: sleeper-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-transactions-api-openapi.yml
- filename: sleeper-users-api-openapi.yml
  format: yaml
  label: Sleeper Users API
  slug: sleeper-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-users-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Sleeper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sleeper secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sleeper
provider_slug: sleeper
scheme_count: 0
schemes: []
slug: sleeper-authentication
source_filename: sleeper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sleeper.com/\ndocs: https://docs.sleeper.com/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The Sleeper API is public and read-only. No API token, API key, or OAuth is\n    required or accepted — the docs state \"you do not need a token to use the\n    Sleeper API\" because no content can be modified through it. Requests are\n    plain HTTPS GET calls. Access control is therefore by IP-based rate limiting\n    (stay under 1,000 requests/minute) rather than authentication.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/authentication/sleeper-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Fantasy Sports
- Sports
- Fantasy Football
- Gaming
- Sports Data
- Leagues
- Consumer
---
