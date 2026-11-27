---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: google-maps-pollen-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Maps Pollen Forecast API
  slug: google-maps-pollen-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-forecast-api-openapi.yml
- filename: google-maps-address-validation-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Address Validation V1 API
  slug: google-maps-address-validation-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-address-validation-v1-api-openapi.yml
- filename: google-maps-air-quality-currentconditions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality CurrentConditions API
  slug: google-maps-air-quality-currentconditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-currentconditions-api-openapi.yml
- filename: google-maps-air-quality-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality Forecast API
  slug: google-maps-air-quality-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-forecast-api-openapi.yml
- filename: google-maps-air-quality-history-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality History API
  slug: google-maps-air-quality-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-history-api-openapi.yml
- filename: google-maps-air-quality-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality MapTypes API
  slug: google-maps-air-quality-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-maptypes-api-openapi.yml
- filename: google-maps-area-insights-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Area Insights V1 API
  slug: google-maps-area-insights-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-area-insights-v1-api-openapi.yml
- filename: google-maps-pollen-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Pollen MapTypes API
  slug: google-maps-pollen-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-maptypes-api-openapi.yml
- filename: google-maps-solar-buildinginsights-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar BuildingInsights API
  slug: google-maps-solar-buildinginsights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-buildinginsights-api-openapi.yml
- filename: google-maps-solar-datalayers-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar DataLayers API
  slug: google-maps-solar-datalayers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-datalayers-api-openapi.yml
- filename: google-maps-solar-geotiff-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar GeoTiff API
  slug: google-maps-solar-geotiff-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-geotiff-api-openapi.yml
- filename: google-maps-street-view-publish-photo-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photo API
  slug: google-maps-street-view-publish-photo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photo-api-openapi.yml
- filename: google-maps-street-view-publish-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photos API
  slug: google-maps-street-view-publish-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photos-api-openapi.yml
- filename: google-maps-street-view-publish-photosequence-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequence API
  slug: google-maps-street-view-publish-photosequence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequence-api-openapi.yml
- filename: google-maps-street-view-publish-photosequences-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequences API
  slug: google-maps-street-view-publish-photosequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequences-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Google Maps Platform Authentication
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
