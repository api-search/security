---
api_key_in:
- query
api_specs:
- filename: tomorrow-alerts-api-openapi.yml
  format: yaml
  label: Tomorrow.io Alerts API
  slug: tomorrow-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-alerts-api-openapi.yml
- filename: tomorrow-climate-api-openapi.yml
  format: yaml
  label: Tomorrow.io Climate API
  slug: tomorrow-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-climate-api-openapi.yml
- filename: tomorrow-events-api-openapi.yml
  format: yaml
  label: Tomorrow.io Events API
  slug: tomorrow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-events-api-openapi.yml
- filename: tomorrow-forecast-api-openapi.yml
  format: yaml
  label: Tomorrow.io Forecast API
  slug: tomorrow-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-forecast-api-openapi.yml
- filename: tomorrow-historical-api-openapi.yml
  format: yaml
  label: Tomorrow.io Historical API
  slug: tomorrow-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-historical-api-openapi.yml
- filename: tomorrow-insights-api-openapi.yml
  format: yaml
  label: Tomorrow.io Insights API
  slug: tomorrow-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-insights-api-openapi.yml
- filename: tomorrow-locations-api-openapi.yml
  format: yaml
  label: Tomorrow.io Locations API
  slug: tomorrow-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-locations-api-openapi.yml
- filename: tomorrow-map-tiles-api-openapi.yml
  format: yaml
  label: Tomorrow.io Map Tiles API
  slug: tomorrow-map-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-map-tiles-api-openapi.yml
- filename: tomorrow-realtime-api-openapi.yml
  format: yaml
  label: Tomorrow.io Realtime API
  slug: tomorrow-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-realtime-api-openapi.yml
- filename: tomorrow-routes-api-openapi.yml
  format: yaml
  label: Tomorrow.io Routes API
  slug: tomorrow-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-routes-api-openapi.yml
- filename: tomorrow-timelines-api-openapi.yml
  format: yaml
  label: Tomorrow.io Timelines API
  slug: tomorrow-timelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-timelines-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tomorrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tomorrow.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tomorrow.io
provider_slug: tomorrow
scheme_count: 1
schemes:
- description: Tomorrow.io API key passed as `apikey` query parameter. Obtain at https://app.tomorrow.io/development/keys.
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/tomorrow-openapi.yml
  type: apiKey
slug: tomorrow-authentication
source_filename: tomorrow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tomorrow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Tomorrow.io API key passed as `apikey` query parameter. Obtain at https://app.tomorrow.io/development/keys.\n  sources:\n  - openapi/tomorrow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/authentication/tomorrow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Climate
- Forecast
- Historical Weather
- Air Quality
- Pollen
- Fire
- Flood
- Routes
- Map Tiles
- Aviation
- Maritime
- Public APIs
---
