---
api_key_in:
- header
api_specs:
- filename: radar-io-addresses-api-openapi.yml
  format: yaml
  label: Radar Addresses API
  slug: radar-io-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-addresses-api-openapi.yml
- filename: radar-io-events-api-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-io-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-events-api-openapi.yml
- filename: radar-io-geocoding-api-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-io-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-geocoding-api-openapi.yml
- filename: radar-io-geofences-api-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-io-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-geofences-api-openapi.yml
- filename: radar-io-routing-api-openapi.yml
  format: yaml
  label: Radar Routing API
  slug: radar-io-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-routing-api-openapi.yml
- filename: radar-io-search-api-openapi.yml
  format: yaml
  label: Radar Search API
  slug: radar-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-search-api-openapi.yml
- filename: radar-io-tiles-api-openapi.yml
  format: yaml
  label: Radar Tiles API
  slug: radar-io-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-tiles-api-openapi.yml
- filename: radar-io-track-api-openapi.yml
  format: yaml
  label: Radar Track API
  slug: radar-io-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-track-api-openapi.yml
- filename: radar-io-trips-api-openapi.yml
  format: yaml
  label: Radar Trips API
  slug: radar-io-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-trips-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Radar Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radar
provider_slug: radar-io
scheme_count: 1
schemes:
- description: A Radar publishable (client) key (prj_live_pk_... / prj_test_pk_...) or secret (server) key (prj_live_sk_... / prj_test_sk_...), passed in the Authorization header without a Bearer prefix.
  in: header
  name: RadarKey
  parameter: Authorization
  sources:
  - openapi/radar-io-openapi.yml
  type: apiKey
slug: radar-io-authentication
source_filename: radar-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radar-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RadarKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A Radar publishable (client) key (prj_live_pk_... / prj_test_pk_...) or secret\n    (server) key (prj_live_sk_... / prj_test_sk_...), passed in the Authorization header without\n    a Bearer prefix.\n  sources:\n  - openapi/radar-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/authentication/radar-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Location
- Geocoding
- Geofencing
- Maps
- Routing
---
