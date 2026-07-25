---
api_key_in:
- header
api_specs:
- filename: blablacar-bus-api-bookings-api-openapi.yml
  format: yaml
  label: BlaBlaCar Bus API Bookings API
  slug: blablacar-bus-api-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-bookings-api-openapi.yml
- filename: blablacar-bus-api-routes-api-openapi.yml
  format: yaml
  label: BlaBlaCar Bus API Routes API
  slug: blablacar-bus-api-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-routes-api-openapi.yml
- filename: blablacar-bus-api-stations-api-openapi.yml
  format: yaml
  label: BlaBlaCar Bus API Stations API
  slug: blablacar-bus-api-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-stations-api-openapi.yml
- filename: blablacar-bus-api-tickets-api-openapi.yml
  format: yaml
  label: BlaBlaCar Bus API Tickets API
  slug: blablacar-bus-api-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-tickets-api-openapi.yml
- filename: blablacar-bus-api-trips-api-openapi.yml
  format: yaml
  label: BlaBlaCar Bus API Trips API
  slug: blablacar-bus-api-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-trips-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blablacar Bus Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlaBlaCar Bus API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
scheme_count: 1
schemes:
- description: API key provided by BlaBlaCar Bus partner program
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/blablacar-bus-api-openapi.yaml
  type: apiKey
slug: blablacar-bus-api-authentication
source_filename: blablacar-bus-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blablacar-bus-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key provided by BlaBlaCar Bus partner program\n  sources:\n  - openapi/blablacar-bus-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/authentication/blablacar-bus-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
---
