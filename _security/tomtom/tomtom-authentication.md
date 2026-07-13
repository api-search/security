---
api_key_in:
- query
api_specs:
- filename: tomtom-maps-openapi.yml
  format: yaml
  label: TomTom Maps API
  slug: tomtom-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-maps-openapi.yml
- filename: tomtom-search-openapi.yml
  format: yaml
  label: TomTom Search API
  slug: tomtom-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-search-openapi.yml
- filename: tomtom-routing-openapi.yml
  format: yaml
  label: TomTom Routing API
  slug: tomtom-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-routing-openapi.yml
- filename: tomtom-traffic-openapi.yml
  format: yaml
  label: TomTom Traffic API
  slug: tomtom-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-openapi.yml
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
