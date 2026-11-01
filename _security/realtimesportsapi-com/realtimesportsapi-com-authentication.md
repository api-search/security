---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: realtimesportsapi-com-athletes-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Athletes API
  slug: realtimesportsapi-com-athletes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-athletes-api-openapi.yml
- filename: realtimesportsapi-com-events-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Events API
  slug: realtimesportsapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-events-api-openapi.yml
- filename: realtimesportsapi-com-injuries-availability-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Injuries & Availability API
  slug: realtimesportsapi-com-injuries-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-injuries-availability-api-openapi.yml
- filename: realtimesportsapi-com-news-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com News API
  slug: realtimesportsapi-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-news-api-openapi.yml
- filename: realtimesportsapi-com-odds-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Odds API
  slug: realtimesportsapi-com-odds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-odds-api-openapi.yml
- filename: realtimesportsapi-com-plays-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Plays API
  slug: realtimesportsapi-com-plays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-plays-api-openapi.yml
- filename: realtimesportsapi-com-seasons-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Seasons API
  slug: realtimesportsapi-com-seasons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-seasons-api-openapi.yml
- filename: realtimesportsapi-com-sports-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Sports API
  slug: realtimesportsapi-com-sports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-sports-api-openapi.yml
- filename: realtimesportsapi-com-teams-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Teams API
  slug: realtimesportsapi-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-teams-api-openapi.yml
- filename: realtimesportsapi-com-transactions-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Transactions API
  slug: realtimesportsapi-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-transactions-api-openapi.yml
- filename: realtimesportsapi-com-webhooks-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com Webhooks API
  slug: realtimesportsapi-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-webhooks-api-openapi.yml
- filename: realtimesportsapi-com-websocket-api-openapi.yml
  format: yaml
  label: realtimesportsapi-com WebSocket API
  slug: realtimesportsapi-com-websocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realtimesportsapi-com/openapi/realtimesportsapi-com-websocket-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Realtimesportsapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: realtimesportsapi-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: realtimesportsapi-com
provider_slug: realtimesportsapi-com
scheme_count: 2
schemes:
- description: 'Your API key from the dashboard: `Authorization: Bearer <api key>`. Keys are opaque strings, not JWTs.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/original.json
  - openapi/realtimesportsapi-com-openapi.json
  type: http
- description: Alternative to the Authorization header (useful behind proxies that strip Authorization).
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/original.json
  - openapi/realtimesportsapi-com-openapi.json
  type: apiKey
slug: realtimesportsapi-com-authentication
source_filename: realtimesportsapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/original.json, openapi/realtimesportsapi-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Your API key from the dashboard: `Authorization: Bearer <api key>`. Keys are\n    opaque strings, not JWTs.'\n  sources:\n  - openapi/original.json\n  - openapi/realtimesportsapi-com-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative to the Authorization header (useful behind proxies that strip Authorization).\n  sources:\n  - openapi/original.json\n  - openapi/realtimesportsapi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/realtimesportsapi-com/authentication/realtimesportsapi-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sports
- API
- Real-time
- Betting
---
