---
api_key_in:
- query
api_specs:
- filename: opentripmap-openapi.json
  format: json
  label: OpenTripMap API
  slug: opentripmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentripmap/refs/heads/main/openapi/opentripmap-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opentripmap Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenTripMap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenTripMap
provider_slug: opentripmap
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/opentripmap-openapi.json
  type: apiKey
slug: opentripmap-authentication
source_filename: opentripmap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opentripmap-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/opentripmap-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentripmap/refs/heads/main/authentication/opentripmap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel
- Points of Interest
- POI
- Tourism
- Maps
- Geospatial
- OpenStreetMap
- Wikipedia
- Attractions
- Restaurants
- Hotels
- Museums
- REST API
---
