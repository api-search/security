---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: google-maps-autocomplete-api-openapi.yml
  format: yaml
  label: Google Maps Platform Autocomplete API
  slug: google-maps-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-autocomplete-api-openapi.yml
- filename: google-maps-directions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-openapi.yml
- filename: google-maps-geocoding-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-openapi.yml
- filename: google-maps-nearby-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Nearby Search API
  slug: google-maps-nearby-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-nearby-search-api-openapi.yml
- filename: google-maps-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Photos API
  slug: google-maps-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-photos-api-openapi.yml
- filename: google-maps-place-details-api-openapi.yml
  format: yaml
  label: Google Maps Platform Place Details API
  slug: google-maps-place-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-place-details-api-openapi.yml
- filename: google-maps-text-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Text Search API
  slug: google-maps-text-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-text-search-api-openapi.yml
- filename: google-maps-directions-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-api-openapi.yml
- filename: google-maps-distance-matrix-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Distance Matrix API
  slug: google-maps-distance-matrix-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-distance-matrix-api-api-openapi.yml
- filename: google-maps-elevation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Elevation API
  slug: google-maps-elevation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-elevation-api-api-openapi.yml
- filename: google-maps-geocoding-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-api-openapi.yml
- filename: google-maps-geolocation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geolocation API
  slug: google-maps-geolocation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geolocation-api-api-openapi.yml
- filename: google-maps-places-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Places API
  slug: google-maps-places-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-places-api-api-openapi.yml
- filename: google-maps-roads-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Roads API
  slug: google-maps-roads-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-roads-api-api-openapi.yml
- filename: google-maps-street-view-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View API
  slug: google-maps-street-view-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-api-api-openapi.yml
- filename: google-maps-time-zone-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Time Zone API
  slug: google-maps-time-zone-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-time-zone-api-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: openapi/google-maps-directions-api.yml, openapi/google-maps-geocoding-api.yml,\n  openapi/google-maps-places-api.yml\ndocs: https://developers.google.com/maps/documentation/javascript/get-api-key\noauth2_docs: https://developers.google.com/maps/documentation/places/web-service/get-api-key\nnote: 'Primary auth is a Google Maps Platform API key delivered as the `key` query\n  parameter (legacy web-service APIs) or the `X-Goog-Api-Key` header (newer googleapis.com\n  endpoints). A subset of Cloud-based services (Route Optimization, Maps Datasets,\n  Address Validation, Aerial View, Places Insights) additionally accept OAuth 2.0\n  access tokens / service-account credentials via Google Cloud. Keys are created and\n  restricted in the Google Cloud console. (2026-11-05: the previous oauth2_docs URL,\n  .../route-optimization/auth, returned HTTP 404; replaced with the Places API (New)\n  setup page, which documents the OAuth scope.)'\n\
  summary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Google Maps Platform API key\n  sources:\n  - openapi/google-maps-directions-api.yml\n  - openapi/google-maps-geocoding-api.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Goog-Api-Key\n  description: Google Maps Platform API key\n  sources:\n  - openapi/google-maps-places-api.yml\noauth2_scope: https://www.googleapis.com/auth/cloud-platform\n"
source_yaml_url: https://artifacts.apis.io/google-maps/authentication/google-maps-authentication.yml
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
- Geospatial
---
