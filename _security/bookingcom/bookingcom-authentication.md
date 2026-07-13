---
api_key_in: []
api_specs:
- filename: bookingcom-booking-api-openapi.yml
  format: yaml
  label: Booking.com API
  slug: booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookingcom/refs/heads/main/openapi/bookingcom-booking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bookingcom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booking.com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Booking.com
provider_slug: bookingcom
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bookingcom-booking-api-openapi.yml
  type: http
slug: bookingcom-authentication
source_filename: bookingcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bookingcom-booking-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bookingcom-booking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookingcom/refs/heads/main/authentication/bookingcom-authentication.yml
summary_line: http · 1 scheme
tags:
- Accommodations
- Affiliates
- Connectivity
- Hospitality
- Hotels
- Reservations
- Travel
---
