---
api_key_in:
- header
api_specs:
- filename: ors
  format: yaml
  label: OpenRouteService Directions API
  slug: directions
  spec_type: OpenAPI
  url: https://openrouteservice.org/wp-json/ors
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openrouteservice Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRouteService secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRouteService
provider_slug: openrouteservice
scheme_count: 1
schemes:
- description: API key obtained from https://openrouteservice.org
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/openrouteservice-openapi.yml
  type: apiKey
slug: openrouteservice-authentication
source_filename: openrouteservice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openrouteservice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key obtained from https://openrouteservice.org\n  sources:\n  - openapi/openrouteservice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/authentication/openrouteservice-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Routing
- Geospatial
- Directions
- Isochrones
- Matrix
- Geocoding
- Elevation
- Optimization
- OpenStreetMap
- Navigation
- Logistics
- Humanitarian
---
