---
api_key_in:
- header
api_specs:
- filename: radar-events-api-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-events-api-openapi.yml
- filename: radar-geocoding-api-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-geocoding-api-openapi.yml
- filename: radar-geofences-api-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-geofences-api-openapi.yml
- filename: radar-routing-api-openapi.yml
  format: yaml
  label: Radar Routing API
  slug: radar-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-routing-api-openapi.yml
- filename: radar-search-api-openapi.yml
  format: yaml
  label: Radar Search API
  slug: radar-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-search-api-openapi.yml
- filename: radar-track-api-openapi.yml
  format: yaml
  label: Radar Track API
  slug: radar-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-track-api-openapi.yml
- filename: radar-users-api-openapi.yml
  format: yaml
  label: Radar Users API
  slug: radar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radar
provider_slug: radar
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/radar-openapi.yml
  type: apiKey
slug: radar-authentication
source_filename: radar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radar-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/radar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/authentication/radar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Location
- Geocoding
- Geofencing
- Routing
- Maps
---
