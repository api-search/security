---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chartmetric-charts-api-openapi.yml
  format: yaml
  label: Chartmetric Charts API
  slug: chartmetric-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-charts-api-openapi.yml
- filename: chartmetric-search-api-openapi.yml
  format: yaml
  label: Chartmetric Search API
  slug: chartmetric-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-search-api-openapi.yml
- filename: chartmetric-album-api-openapi.yml
  format: yaml
  label: Chartmetric Album API
  slug: chartmetric-album-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-album-api-openapi.yml
- filename: chartmetric-artist-api-openapi.yml
  format: yaml
  label: Chartmetric Artist API
  slug: chartmetric-artist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-artist-api-openapi.yml
- filename: chartmetric-brand-api-openapi.yml
  format: yaml
  label: Chartmetric Brand API
  slug: chartmetric-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-brand-api-openapi.yml
- filename: chartmetric-city-api-openapi.yml
  format: yaml
  label: Chartmetric City API
  slug: chartmetric-city-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-city-api-openapi.yml
- filename: chartmetric-country-api-openapi.yml
  format: yaml
  label: Chartmetric Country API
  slug: chartmetric-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-country-api-openapi.yml
- filename: chartmetric-curator-api-openapi.yml
  format: yaml
  label: Chartmetric Curator API
  slug: chartmetric-curator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-curator-api-openapi.yml
- filename: chartmetric-event-api-openapi.yml
  format: yaml
  label: Chartmetric Event API
  slug: chartmetric-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-event-api-openapi.yml
- filename: chartmetric-festival-api-openapi.yml
  format: yaml
  label: Chartmetric Festival API
  slug: chartmetric-festival-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-festival-api-openapi.yml
- filename: chartmetric-genre-api-openapi.yml
  format: yaml
  label: Chartmetric Genre API
  slug: chartmetric-genre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-genre-api-openapi.yml
- filename: chartmetric-playlist-api-openapi.yml
  format: yaml
  label: Chartmetric Playlist API
  slug: chartmetric-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-playlist-api-openapi.yml
- filename: chartmetric-radio-api-openapi.yml
  format: yaml
  label: Chartmetric Radio API
  slug: chartmetric-radio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-radio-api-openapi.yml
- filename: chartmetric-sns-api-openapi.yml
  format: yaml
  label: Chartmetric SNS API
  slug: chartmetric-sns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-sns-api-openapi.yml
- filename: chartmetric-token-api-openapi.yml
  format: yaml
  label: Chartmetric Token API
  slug: chartmetric-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-token-api-openapi.yml
- filename: chartmetric-track-api-openapi.yml
  format: yaml
  label: Chartmetric Track API
  slug: chartmetric-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-track-api-openapi.yml
- filename: chartmetric-venue-api-openapi.yml
  format: yaml
  label: Chartmetric Venue API
  slug: chartmetric-venue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-venue-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chartmetric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chartmetric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chartmetric
provider_slug: chartmetric
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token obtained from POST /token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chartmetric-openapi.yml
  type: http
slug: chartmetric-authentication
source_filename: chartmetric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chartmetric-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token obtained from POST /token.\n  sources:\n  - openapi/chartmetric-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/chartmetric/authentication/chartmetric-authentication.yml
summary_line: http · 1 scheme
tags:
- Music
- Analytics
- Artist Intelligence
- Streaming
- Charts
---
