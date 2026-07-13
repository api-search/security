---
api_key_in:
- query
api_specs:
- filename: tomorrow-io-weather-api-openapi.yml
  format: yaml
  label: Tomorrow.io Weather API
  slug: tomorrow-io-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-weather-api-openapi.yml
- filename: tomorrow-io-historical-api-openapi.yml
  format: yaml
  label: Tomorrow.io Historical Weather API
  slug: tomorrow-io-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-historical-api-openapi.yml
- filename: tomorrow-io-events-api-openapi.yml
  format: yaml
  label: Tomorrow.io Events API
  slug: tomorrow-io-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-events-api-openapi.yml
- filename: tomorrow-io-route-api-openapi.yml
  format: yaml
  label: Tomorrow.io Weather on Routes API
  slug: tomorrow-io-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-route-api-openapi.yml
- filename: tomorrow-io-map-tiles-api-openapi.yml
  format: yaml
  label: Tomorrow.io Weather Maps API
  slug: tomorrow-io-map-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-map-tiles-api-openapi.yml
- filename: tomorrow-io-locations-api-openapi.yml
  format: yaml
  label: Tomorrow.io Locations API
  slug: tomorrow-io-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-locations-api-openapi.yml
- filename: tomorrow-io-alerts-api-openapi.yml
  format: yaml
  label: Tomorrow.io Alerts API
  slug: tomorrow-io-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-alerts-api-openapi.yml
- filename: tomorrow-io-insights-api-openapi.yml
  format: yaml
  label: Tomorrow.io Insights API
  slug: tomorrow-io-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/openapi/tomorrow-io-insights-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tomorrow Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tomorrow.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tomorrow.io
provider_slug: tomorrow-io
scheme_count: 1
schemes:
- in: query
  name: apikeyAuth
  parameter: apikey
  sources:
  - openapi/tomorrow-io-alerts-api-openapi.yml
  - openapi/tomorrow-io-events-api-openapi.yml
  - openapi/tomorrow-io-historical-api-openapi.yml
  - openapi/tomorrow-io-insights-api-openapi.yml
  - openapi/tomorrow-io-locations-api-openapi.yml
  - openapi/tomorrow-io-map-tiles-api-openapi.yml
  - openapi/tomorrow-io-route-api-openapi.yml
  - openapi/tomorrow-io-weather-api-openapi.yml
  type: apiKey
slug: tomorrow-io-authentication
source_filename: tomorrow-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tomorrow-io-alerts-api-openapi.yml, openapi/tomorrow-io-events-api-openapi.yml,\n  openapi/tomorrow-io-historical-api-openapi.yml, openapi/tomorrow-io-insights-api-openapi.yml,\n  openapi/tomorrow-io-locations-api-openapi.yml, openapi/tomorrow-io-map-tiles-api-openapi.yml,\n  openapi/tomorrow-io-route-api-openapi.yml, openapi/tomorrow-io-weather-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/tomorrow-io-alerts-api-openapi.yml\n  - openapi/tomorrow-io-events-api-openapi.yml\n  - openapi/tomorrow-io-historical-api-openapi.yml\n  - openapi/tomorrow-io-insights-api-openapi.yml\n  - openapi/tomorrow-io-locations-api-openapi.yml\n  - openapi/tomorrow-io-map-tiles-api-openapi.yml\n  - openapi/tomorrow-io-route-api-openapi.yml\n  - openapi/tomorrow-io-weather-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/authentication/tomorrow-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Forecast
- Climate
- Risk
- Air Quality
- Pollen
- Lightning
- Severe Weather
- Maps
- Routing
- Satellite
- Microsatellites
- Radar
- Geospatial
- Alerts
---
