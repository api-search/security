---
api_key_in:
- header
api_specs:
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Search & Autocomplete API
  slug: radar-search-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Routing, Distance & Matrix API
  slug: radar-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Track & Users API
  slug: radar-track-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Trips API
  slug: radar-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Address Verification API
  slug: radar-address-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Maps & Tiles API
  slug: radar-maps-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
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
