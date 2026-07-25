---
api_key_in:
- header
- query
api_specs:
- filename: mbta-alerts-api-openapi.yml
  format: yaml
  label: MBTA Alerts API
  slug: mbta-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-alerts-api-openapi.yml
- filename: mbta-facilities-api-openapi.yml
  format: yaml
  label: MBTA Facilities API
  slug: mbta-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-facilities-api-openapi.yml
- filename: mbta-lines-api-openapi.yml
  format: yaml
  label: MBTA Lines API
  slug: mbta-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-lines-api-openapi.yml
- filename: mbta-predictions-api-openapi.yml
  format: yaml
  label: MBTA Predictions API
  slug: mbta-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-predictions-api-openapi.yml
- filename: mbta-routepatterns-api-openapi.yml
  format: yaml
  label: MBTA RoutePatterns API
  slug: mbta-routepatterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routepatterns-api-openapi.yml
- filename: mbta-routes-api-openapi.yml
  format: yaml
  label: MBTA Routes API
  slug: mbta-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routes-api-openapi.yml
- filename: mbta-schedules-api-openapi.yml
  format: yaml
  label: MBTA Schedules API
  slug: mbta-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-schedules-api-openapi.yml
- filename: mbta-services-api-openapi.yml
  format: yaml
  label: MBTA Services API
  slug: mbta-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-services-api-openapi.yml
- filename: mbta-shapes-api-openapi.yml
  format: yaml
  label: MBTA Shapes API
  slug: mbta-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-shapes-api-openapi.yml
- filename: mbta-stops-api-openapi.yml
  format: yaml
  label: MBTA Stops API
  slug: mbta-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-stops-api-openapi.yml
- filename: mbta-trips-api-openapi.yml
  format: yaml
  label: MBTA Trips API
  slug: mbta-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-trips-api-openapi.yml
- filename: mbta-vehicles-api-openapi.yml
  format: yaml
  label: MBTA Vehicles API
  slug: mbta-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-vehicles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mbta Authentication
name_suffix: Authentication
oauth_flows: []
overview: MBTA secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MBTA
provider_slug: mbta
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/mbta-mbta-v3-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/mbta-mbta-v3-api-openapi.yml
  type: apiKey
slug: mbta-authentication
source_filename: mbta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mbta-mbta-v3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/mbta-mbta-v3-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/mbta-mbta-v3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/authentication/mbta-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Boston
- Massachusetts
- Public Transportation
- Real-Time
- Transit
---
