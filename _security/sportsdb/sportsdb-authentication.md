---
api_key_in:
- header
api_specs:
- filename: sportsdb-events-api-openapi.yml
  format: yaml
  label: TheSportsDB Events API
  slug: sportsdb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-events-api-openapi.yml
- filename: sportsdb-leagues-api-openapi.yml
  format: yaml
  label: TheSportsDB Leagues API
  slug: sportsdb-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-leagues-api-openapi.yml
- filename: sportsdb-livescores-api-openapi.yml
  format: yaml
  label: TheSportsDB Livescores API
  slug: sportsdb-livescores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-livescores-api-openapi.yml
- filename: sportsdb-lookup-api-openapi.yml
  format: yaml
  label: TheSportsDB Lookup API
  slug: sportsdb-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-lookup-api-openapi.yml
- filename: sportsdb-players-api-openapi.yml
  format: yaml
  label: TheSportsDB Players API
  slug: sportsdb-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-players-api-openapi.yml
- filename: sportsdb-search-api-openapi.yml
  format: yaml
  label: TheSportsDB Search API
  slug: sportsdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-search-api-openapi.yml
- filename: sportsdb-teams-api-openapi.yml
  format: yaml
  label: TheSportsDB Teams API
  slug: sportsdb-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-teams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportsdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheSportsDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TheSportsDB
provider_slug: sportsdb
scheme_count: 1
schemes:
- description: Premium V2 API key supplied in the X-API-KEY request header.
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/sportsdb-openapi.yml
  type: apiKey
slug: sportsdb-authentication
source_filename: sportsdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportsdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Premium V2 API key supplied in the X-API-KEY request header.\n  sources:\n  - openapi/sportsdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/authentication/sportsdb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Sports Data
- Teams
- Players
- Events
---
