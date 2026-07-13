---
api_key_in: []
api_specs:
- filename: booking-com-demand-api.yaml
  format: yaml
  label: Booking.com Demand API
  slug: bookingcom-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-com-demand-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Booking Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booking Holdings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Booking Holdings
provider_slug: booking-holdings
scheme_count: 1
schemes:
- bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/booking-com-demand-api.yaml
  type: http
slug: booking-holdings-authentication
source_filename: booking-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/booking-com-demand-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  sources:\n  - openapi/booking-com-demand-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/authentication/booking-holdings-authentication.yml
summary_line: http · 1 scheme
tags:
- Accommodations
- Airlines
- Car Rentals
- Hospitality
- Hotels
- Restaurants
- Travel
---
