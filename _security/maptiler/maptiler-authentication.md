---
api_key_in:
- query
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
