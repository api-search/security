---
api_key_in:
- query
api_specs:
- filename: maptiler-maps-api-openapi.yml
  format: yaml
  label: MapTiler Maps API
  slug: maptiler-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-maps-api-openapi.yml
- filename: maptiler-tiles-api-openapi.yml
  format: yaml
  label: MapTiler Tiles API
  slug: maptiler-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-tiles-api-openapi.yml
- filename: maptiler-geocoding-api-openapi.yml
  format: yaml
  label: MapTiler Geocoding API
  slug: maptiler-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-geocoding-api-openapi.yml
- filename: maptiler-static-maps-api-openapi.yml
  format: yaml
  label: MapTiler Static Maps API
  slug: maptiler-static-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-static-maps-api-openapi.yml
- filename: maptiler-elevation-api-openapi.yml
  format: yaml
  label: MapTiler Elevation API
  slug: maptiler-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-elevation-api-openapi.yml
- filename: maptiler-geolocation-api-openapi.yml
  format: yaml
  label: MapTiler Geolocation API
  slug: maptiler-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-geolocation-api-openapi.yml
- filename: maptiler-coordinates-api-openapi.yml
  format: yaml
  label: MapTiler Coordinates API
  slug: maptiler-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-coordinates-api-openapi.yml
- filename: maptiler-coordinates-api-openapi.yml
  format: yaml
  label: MapTiler Coordinates API
  slug: maptiler-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-coordinates-api-openapi.yml
- filename: maptiler-data-api-openapi.yml
  format: yaml
  label: MapTiler Data API
  slug: maptiler-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-data-api-openapi.yml
- filename: maptiler-elevation-api-openapi.yml
  format: yaml
  label: MapTiler Elevation API
  slug: maptiler-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-elevation-api-openapi.yml
- filename: maptiler-geocoding-api-openapi.yml
  format: yaml
  label: MapTiler Geocoding API
  slug: maptiler-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-geocoding-api-openapi.yml
- filename: maptiler-geolocation-api-openapi.yml
  format: yaml
  label: MapTiler Geolocation API
  slug: maptiler-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-geolocation-api-openapi.yml
- filename: maptiler-images-api-openapi.yml
  format: yaml
  label: MapTiler Images API
  slug: maptiler-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-images-api-openapi.yml
- filename: maptiler-maps-api-openapi.yml
  format: yaml
  label: MapTiler Maps API
  slug: maptiler-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-maps-api-openapi.yml
- filename: maptiler-other-api-openapi.yml
  format: yaml
  label: MapTiler Other API
  slug: maptiler-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-other-api-openapi.yml
- filename: maptiler-static-maps-api-openapi.yml
  format: yaml
  label: MapTiler Static maps API
  slug: maptiler-static-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-static-maps-api-openapi.yml
- filename: maptiler-tiles-api-openapi.yml
  format: yaml
  label: MapTiler Tiles API
  slug: maptiler-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-tiles-api-openapi.yml
- filename: maptiler-weather-api-openapi.yml
  format: yaml
  label: MapTiler Weather API
  slug: maptiler-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/openapi/maptiler-weather-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Maptiler Authentication
name_suffix: Authentication
oauth_flows: []
overview: MapTiler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MapTiler
provider_slug: maptiler
scheme_count: 1
schemes:
- description: Your own API key from https://cloud.maptiler.com/
  in: query
  name: key
  parameter: key
  sources:
  - openapi/maptiler-maptiler-openapi.yml
  type: apiKey
slug: maptiler-authentication
source_filename: maptiler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maptiler-maptiler-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: key\n  type: apiKey\n  in: query\n  parameter: key\n  description: Your own API key from https://cloud.maptiler.com/\n  sources:\n  - openapi/maptiler-maptiler-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maptiler/refs/heads/main/authentication/maptiler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Maps
- Geospatial
- Tiles
- Vector Tiles
- Satellite Imagery
- Geocoding
- Reverse Geocoding
- Static Maps
- Elevation
- Geolocation
- Coordinate Transformation
- GIS
- Mapping Platform
---
