---
api_key_in:
- header
api_specs:
- filename: unrivaled-basketball-games-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Games API
  slug: unrivaled-basketball-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-games-api-openapi.yml
- filename: unrivaled-basketball-league-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball League API
  slug: unrivaled-basketball-league-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-league-api-openapi.yml
- filename: unrivaled-basketball-players-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Players API
  slug: unrivaled-basketball-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-players-api-openapi.yml
- filename: unrivaled-basketball-seasons-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Seasons API
  slug: unrivaled-basketball-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-seasons-api-openapi.yml
- filename: unrivaled-basketball-series-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Series API
  slug: unrivaled-basketball-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-series-api-openapi.yml
- filename: unrivaled-basketball-teams-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Teams API
  slug: unrivaled-basketball-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-teams-api-openapi.yml
- filename: unrivaled-basketball-tournaments-api-openapi.yml
  format: yaml
  label: Unrivaled Basketball Tournaments API
  slug: unrivaled-basketball-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-tournaments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unrivaled Basketball Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unrivaled Basketball secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unrivaled Basketball
provider_slug: unrivaled-basketball
scheme_count: 1
schemes:
- access_levels:
  - trial
  - production
  in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/unrivaled-basketball-openapi.yml
  type: apiKey
slug: unrivaled-basketball-authentication
source_filename: unrivaled-basketball-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unrivaled-basketball-openapi.yml\ndocs: https://developer.sportradar.com/basketball/docs/unrivaled-ig-api-basics\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Authentication is required for all Unrivaled API calls. The API is operated\n  by Sportradar as the league's Official Data Provider; HTTP requests are\n  made using the API authentication access established in a Sportradar\n  account. The key is sent in the `x-api-key` header, and the key's access\n  level (`trial` or `production`) is also encoded as the first path segment\n  of every request. Applications must support TLS 1.2 or above.\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  access_levels:\n  - trial\n  - production\n  sources:\n  - openapi/unrivaled-basketball-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/authentication/unrivaled-basketball-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Basketball
- Sports
- Womens Sports
- Sports Data
- Media
- League
---
