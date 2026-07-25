---
api_key_in:
- header
api_specs:
- filename: openrouteservice-directions-api-openapi.yml
  format: yaml
  label: OpenRouteService Directions API
  slug: openrouteservice-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-directions-api-openapi.yml
- filename: openrouteservice-elevation-api-openapi.yml
  format: yaml
  label: OpenRouteService Elevation API
  slug: openrouteservice-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-elevation-api-openapi.yml
- filename: openrouteservice-geocoding-api-openapi.yml
  format: yaml
  label: OpenRouteService Geocoding API
  slug: openrouteservice-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-geocoding-api-openapi.yml
- filename: openrouteservice-health-api-openapi.yml
  format: yaml
  label: OpenRouteService Health API
  slug: openrouteservice-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-health-api-openapi.yml
- filename: openrouteservice-isochrones-api-openapi.yml
  format: yaml
  label: OpenRouteService Isochrones API
  slug: openrouteservice-isochrones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-isochrones-api-openapi.yml
- filename: openrouteservice-matrix-api-openapi.yml
  format: yaml
  label: OpenRouteService Matrix API
  slug: openrouteservice-matrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-matrix-api-openapi.yml
- filename: openrouteservice-optimization-api-openapi.yml
  format: yaml
  label: OpenRouteService Optimization API
  slug: openrouteservice-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-optimization-api-openapi.yml
- filename: openrouteservice-poi-api-openapi.yml
  format: yaml
  label: OpenRouteService POI API
  slug: openrouteservice-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-poi-api-openapi.yml
- filename: openrouteservice-snapping-api-openapi.yml
  format: yaml
  label: OpenRouteService Snapping API
  slug: openrouteservice-snapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-snapping-api-openapi.yml
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
