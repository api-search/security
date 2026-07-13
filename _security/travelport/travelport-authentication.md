---
api_key_in: []
api_specs:
- filename: travelport-openapi.yml
  format: yaml
  label: Travelport TripServices Flights API
  slug: trip-services-flights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Travelport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Travelport secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Travelport
provider_slug: travelport
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Travelport-issued JWT bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/travelport-openapi.yml
  type: http
slug: travelport-authentication
source_filename: travelport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travelport-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Travelport-issued JWT bearer token in the Authorization header.\n  sources:\n  - openapi/travelport-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/authentication/travelport-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Travel Technology
- Reservations
- GDS
- NDC
- Flights
- Hotels
- Payments
---
