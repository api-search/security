---
api_key_in:
- query
api_specs:
- filename: jawg-maps-isochrone-api-openapi.yml
  format: yaml
  label: Jawg Maps Isochrone API
  slug: jawg-maps-isochrone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-isochrone-api-openapi.yml
- filename: jawg-maps-matrix-api-openapi.yml
  format: yaml
  label: Jawg Maps Matrix API
  slug: jawg-maps-matrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-matrix-api-openapi.yml
- filename: jawg-maps-places-api-openapi.yml
  format: yaml
  label: Jawg Maps Places API
  slug: jawg-maps-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-places-api-openapi.yml
- filename: jawg-maps-routing-api-openapi.yml
  format: yaml
  label: Jawg Maps Routing API
  slug: jawg-maps-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-routing-api-openapi.yml
- filename: jawg-maps-static-maps-api-openapi.yml
  format: yaml
  label: Jawg Maps Static Maps API
  slug: jawg-maps-static-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-static-maps-api-openapi.yml
- filename: jawg-maps-styles-api-openapi.yml
  format: yaml
  label: Jawg Maps Styles API
  slug: jawg-maps-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-styles-api-openapi.yml
- filename: jawg-maps-tiles-api-openapi.yml
  format: yaml
  label: Jawg Maps Tiles API
  slug: jawg-maps-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-tiles-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jawg Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jawg Maps secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jawg Maps
provider_slug: jawg-maps
scheme_count: 2
schemes:
- description: Jawg access token, obtained from the Jawg App account.
  in: query
  name: accessToken
  parameter: access-token
  sources:
  - openapi/jawg-maps-openapi.yml
  type: apiKey
- description: Jawg access token supplied as a Bearer token on api.jawg.io surfaces.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jawg-maps-openapi.yml
  type: http
slug: jawg-maps-authentication
source_filename: jawg-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jawg-maps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: access-token\n  description: Jawg access token, obtained from the Jawg App account.\n  sources:\n  - openapi/jawg-maps-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Jawg access token supplied as a Bearer token on api.jawg.io surfaces.\n  sources:\n  - openapi/jawg-maps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/authentication/jawg-maps-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Maps
- Geospatial
- Tiles
- Geocoding
- Routing
- Location
---
