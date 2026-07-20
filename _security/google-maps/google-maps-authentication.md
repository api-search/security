---
api_key_in:
- header
- query
api_specs:
- filename: maps-js.yaml
  format: yaml
  label: Maps JavaScript API
  slug: maps-javascript-api
  spec_type: OpenAPI
  url: https://api.example.com/openapi/maps-js.yaml
- filename: google-maps-geocoding-api.yml
  format: yaml
  label: Geocoding API
  slug: geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-geocoding-api.yml
- filename: google-maps-places-api.yml
  format: yaml
  label: Places API (New)
  slug: places-api-new
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-places-api.yml
- filename: google-maps-directions-api.yml
  format: yaml
  label: Directions API
  slug: directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-directions-api.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Maps Platform secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Google Maps Platform
provider_slug: google-maps
scheme_count: 2
schemes:
- description: Google Maps Platform API key
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-maps-directions-api.yml
  - openapi/google-maps-geocoding-api.yml
  type: apiKey
- description: Google Maps Platform API key
  in: header
  name: apiKey
  parameter: X-Goog-Api-Key
  sources:
  - openapi/google-maps-places-api.yml
  type: apiKey
slug: google-maps-authentication
source_filename: google-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-maps-directions-api.yml, openapi/google-maps-geocoding-api.yml, openapi/google-maps-places-api.yml\ndocs: https://developers.google.com/maps/documentation/javascript/get-api-key\noauth2_docs: https://developers.google.com/maps/documentation/route-optimization/auth\nnote: >-\n  Primary auth is a Google Maps Platform API key delivered as the `key` query parameter\n  (legacy web-service APIs) or the `X-Goog-Api-Key` header (newer googleapis.com endpoints).\n  A subset of Cloud-based services (Route Optimization, Maps Datasets, Address Validation,\n  Aerial View, Places Insights) additionally accept OAuth 2.0 access tokens / service-account\n  credentials via Google Cloud. Keys are created and restricted in the Google Cloud console.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Google Maps\
  \ Platform API key\n  sources:\n  - openapi/google-maps-directions-api.yml\n  - openapi/google-maps-geocoding-api.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Goog-Api-Key\n  description: Google Maps Platform API key\n  sources:\n  - openapi/google-maps-places-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/authentication/google-maps-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
---
