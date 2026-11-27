---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datasportsapi-catalog-api-openapi.yml
  format: yaml
  label: DataSportsAPI Catalog API
  slug: datasportsapi-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-catalog-api-openapi.yml
- filename: datasportsapi-discovery-api-openapi.yml
  format: yaml
  label: DataSportsAPI Discovery API
  slug: datasportsapi-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-discovery-api-openapi.yml
- filename: datasportsapi-exports-api-openapi.yml
  format: yaml
  label: DataSportsAPI Exports API
  slug: datasportsapi-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-exports-api-openapi.yml
- filename: datasportsapi-fixtures-api-openapi.yml
  format: yaml
  label: DataSportsAPI Fixtures API
  slug: datasportsapi-fixtures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-fixtures-api-openapi.yml
- filename: datasportsapi-leagues-api-openapi.yml
  format: yaml
  label: DataSportsAPI Leagues API
  slug: datasportsapi-leagues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-leagues-api-openapi.yml
- filename: datasportsapi-livescores-api-openapi.yml
  format: yaml
  label: DataSportsAPI Livescores API
  slug: datasportsapi-livescores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-livescores-api-openapi.yml
- filename: datasportsapi-odds-api-openapi.yml
  format: yaml
  label: DataSportsAPI Odds API
  slug: datasportsapi-odds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-odds-api-openapi.yml
- filename: datasportsapi-people-api-openapi.yml
  format: yaml
  label: DataSportsAPI People API
  slug: datasportsapi-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-people-api-openapi.yml
- filename: datasportsapi-players-api-openapi.yml
  format: yaml
  label: DataSportsAPI Players API
  slug: datasportsapi-players-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-players-api-openapi.yml
- filename: datasportsapi-races-api-openapi.yml
  format: yaml
  label: DataSportsAPI Races API
  slug: datasportsapi-races-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-races-api-openapi.yml
- filename: datasportsapi-search-api-openapi.yml
  format: yaml
  label: DataSportsAPI Search API
  slug: datasportsapi-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-search-api-openapi.yml
- filename: datasportsapi-teams-api-openapi.yml
  format: yaml
  label: DataSportsAPI Teams API
  slug: datasportsapi-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-teams-api-openapi.yml
- filename: datasportsapi-tracking-api-openapi.yml
  format: yaml
  label: DataSportsAPI Tracking API
  slug: datasportsapi-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-tracking-api-openapi.yml
- filename: datasportsapi-venues-api-openapi.yml
  format: yaml
  label: DataSportsAPI Venues API
  slug: datasportsapi-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-venues-api-openapi.yml
- filename: datasportsapi-websocket-api-openapi.yml
  format: yaml
  label: DataSportsAPI WebSocket API
  slug: datasportsapi-websocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasportsapi/openapi/datasportsapi-websocket-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DataSportsAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataSportsAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataSportsAPI
provider_slug: datasportsapi
scheme_count: 1
schemes:
- description: 'Your secret API key: `Authorization: Bearer dsa_live_…`. Publishable widget keys (`dsa_pub_…`) work only for the endpoints widgets read, from the sites registered on them.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datasportsapi-openapi.json
  type: http
slug: datasportsapi-authentication
source_filename: datasportsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/datasportsapi-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Your secret API key: `Authorization: Bearer dsa_live_…`. Publishable widget\n    keys (`dsa_pub_…`) work only for the endpoints widgets read, from the sites registered on\n    them.'\n  sources:\n  - openapi/datasportsapi-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/datasportsapi/authentication/datasportsapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Sports
- Live Data
- Real-Time
- JSON
---
