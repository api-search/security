---
api_key_in:
- query
api_specs:
- filename: tomtom-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Geocoding API
  slug: tomtom-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-geocoding-api-openapi.yml
- filename: tomtom-additional-data-api-openapi.yml
  format: yaml
  label: TomTom Additional Data API
  slug: tomtom-additional-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-additional-data-api-openapi.yml
- filename: tomtom-batch-routing-api-openapi.yml
  format: yaml
  label: TomTom Batch Routing API
  slug: tomtom-batch-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-batch-routing-api-openapi.yml
- filename: tomtom-copyrights-api-openapi.yml
  format: yaml
  label: TomTom Copyrights API
  slug: tomtom-copyrights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-copyrights-api-openapi.yml
- filename: tomtom-filters-api-openapi.yml
  format: yaml
  label: TomTom Filters API
  slug: tomtom-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-filters-api-openapi.yml
- filename: tomtom-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Geocoding API
  slug: tomtom-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-geocoding-api-openapi.yml
- filename: tomtom-raster-api-openapi.yml
  format: yaml
  label: TomTom Raster API
  slug: tomtom-raster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-raster-api-openapi.yml
- filename: tomtom-reachable-range-api-openapi.yml
  format: yaml
  label: TomTom Reachable Range API
  slug: tomtom-reachable-range-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-reachable-range-api-openapi.yml
- filename: tomtom-reverse-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Reverse Geocoding API
  slug: tomtom-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-reverse-geocoding-api-openapi.yml
- filename: tomtom-routing-api-openapi.yml
  format: yaml
  label: TomTom Routing API
  slug: tomtom-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-routing-api-openapi.yml
- filename: tomtom-search-api-openapi.yml
  format: yaml
  label: TomTom Search API
  slug: tomtom-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-search-api-openapi.yml
- filename: tomtom-traffic-flow-api-openapi.yml
  format: yaml
  label: TomTom Traffic Flow API
  slug: tomtom-traffic-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-flow-api-openapi.yml
- filename: tomtom-traffic-incidents-api-openapi.yml
  format: yaml
  label: TomTom Traffic Incidents API
  slug: tomtom-traffic-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-incidents-api-openapi.yml
- filename: tomtom-traffic-tiles-api-openapi.yml
  format: yaml
  label: TomTom Traffic Tiles API
  slug: tomtom-traffic-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-tiles-api-openapi.yml
- filename: tomtom-vector-api-openapi.yml
  format: yaml
  label: TomTom Vector API
  slug: tomtom-vector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-vector-api-openapi.yml
- filename: tomtom-wms-wmts-api-openapi.yml
  format: yaml
  label: TomTom WMS / WMTS API
  slug: tomtom-wms-wmts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-wms-wmts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tomtom Authentication
name_suffix: Authentication
oauth_flows: []
overview: TomTom secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TomTom
provider_slug: tomtom
scheme_count: 1
schemes:
- in: query
  name: api_key
  parameter: key
  sources:
  - openapi/tomtom-maps-openapi.yml
  - openapi/tomtom-routing-openapi.yml
  - openapi/tomtom-search-openapi.yml
  - openapi/tomtom-traffic-openapi.yml
  type: apiKey
slug: tomtom-authentication
source_filename: tomtom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tomtom-maps-openapi.yml, openapi/tomtom-routing-openapi.yml, openapi/tomtom-search-openapi.yml,\n  openapi/tomtom-traffic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/tomtom-maps-openapi.yml\n  - openapi/tomtom-routing-openapi.yml\n  - openapi/tomtom-search-openapi.yml\n  - openapi/tomtom-traffic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/authentication/tomtom-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Maps
- Traffic
- Transportation
- Navigation
- Location
- Geospatial
- Routing
- Geocoding
---
