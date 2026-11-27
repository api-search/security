---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: localselections-com-bracket-api-openapi.yml
  format: yaml
  label: Local Selections Bracket API
  slug: localselections-com-bracket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-bracket-api-openapi.yml
- filename: localselections-com-events-api-openapi.yml
  format: yaml
  label: Local Selections Events API
  slug: localselections-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-events-api-openapi.yml
- filename: localselections-com-groups-api-openapi.yml
  format: yaml
  label: Local Selections Groups API
  slug: localselections-com-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-groups-api-openapi.yml
- filename: localselections-com-introspect-api-openapi.yml
  format: yaml
  label: Local Selections Introspect API
  slug: localselections-com-introspect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-introspect-api-openapi.yml
- filename: localselections-com-movies-api-openapi.yml
  format: yaml
  label: Local Selections Movies API
  slug: localselections-com-movies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-movies-api-openapi.yml
- filename: localselections-com-places-api-openapi.yml
  format: yaml
  label: Local Selections Places API
  slug: localselections-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-places-api-openapi.yml
- filename: localselections-com-search-api-openapi.yml
  format: yaml
  label: Local Selections Search API
  slug: localselections-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-search-api-openapi.yml
- filename: localselections-com-spin-api-openapi.yml
  format: yaml
  label: Local Selections Spin API
  slug: localselections-com-spin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-spin-api-openapi.yml
- filename: localselections-com-surprise-me-api-openapi.yml
  format: yaml
  label: Local Selections Surprise Me API
  slug: localselections-com-surprise-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localselections-com/openapi/localselections-com-surprise-me-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Local Selections Authentication
name_suffix: Authentication
oauth_flows: []
overview: Local Selections secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Local Selections
provider_slug: localselections-com
scheme_count: 1
schemes:
- description: 'A per-caller API key issued via the authenticated (browser-session) POST /api/account/api-keys endpoint. `Authorization: Bearer <key>` is also accepted as an alternative to the X-API-Key header. Each key carries scopes (`all`, or one or more of `spin`/`search`/`surprise_me`/`bracket`/`groups_host`/`groups_join`/`places`/`events`/`movies`) that gate which paths below it may call — see each path''s d'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/localselections-com-openapi.json
  type: apiKey
slug: localselections-com-authentication
source_filename: localselections-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/localselections-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'A per-caller API key issued via the authenticated (browser-session) POST /api/account/api-keys\n    endpoint. `Authorization: Bearer <key>` is also accepted as an alternative to the X-API-Key\n    header. Each key carries scopes (`all`, or one or more of `spin`/`search`/`surprise_me`/`bracket`/`groups_host`/`groups_join`/`places`/`events`/`movies`)\n    that gate which paths below it may call — see each path''s d'\n  sources:\n  - openapi/localselections-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/localselections-com/authentication/localselections-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- DecisionGames
- Location-based
- Entertainment
- Food
---
