---
api_key_in: []
api_specs:
- filename: tictactrip-autocomplete-api-openapi.yml
  format: yaml
  label: TicTacTrip Autocomplete API
  slug: tictactrip-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-autocomplete-api-openapi.yml
- filename: tictactrip-booking-api-openapi.yml
  format: yaml
  label: TicTacTrip Booking API
  slug: tictactrip-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-booking-api-openapi.yml
- filename: tictactrip-cities-api-openapi.yml
  format: yaml
  label: TicTacTrip Cities API
  slug: tictactrip-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-cities-api-openapi.yml
- filename: tictactrip-results-api-openapi.yml
  format: yaml
  label: TicTacTrip Results API
  slug: tictactrip-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-results-api-openapi.yml
- filename: tictactrip-segmentproviders-api-openapi.yml
  format: yaml
  label: TicTacTrip SegmentProviders API
  slug: tictactrip-segmentproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-segmentproviders-api-openapi.yml
- filename: tictactrip-stopclusters-api-openapi.yml
  format: yaml
  label: TicTacTrip StopClusters API
  slug: tictactrip-stopclusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-stopclusters-api-openapi.yml
- filename: tictactrip-stopgroups-api-openapi.yml
  format: yaml
  label: TicTacTrip StopGroups API
  slug: tictactrip-stopgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-stopgroups-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tictactrip Authentication
name_suffix: Authentication
oauth_flows: []
overview: TicTacTrip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TicTacTrip
provider_slug: tictactrip
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: authentication
  scheme: bearer
  sources:
  - openapi/tictactrip-openapi-original.json
  type: http
slug: tictactrip-authentication
source_filename: tictactrip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tictactrip-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: authentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tictactrip-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/authentication/tictactrip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Travel
- Transportation
- Trains
- Bus
- Booking
- Mobility
- Multi-Modal
- Ticketing
---
