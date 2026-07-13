---
api_key_in:
- header
api_specs:
- filename: booking-com-demand-api-openapi.yml
  format: yaml
  label: Booking.com Demand API
  slug: demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-demand-api-openapi.yml
- filename: booking-com-car-rentals-api-openapi.yml
  format: yaml
  label: Booking.com Car Rentals API
  slug: car-rentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-car-rentals-api-openapi.yml
- filename: booking-com-connectivity-content-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Content API
  slug: connectivity-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-content-api-openapi.yml
- filename: booking-com-connectivity-reservations-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Reservations API
  slug: connectivity-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-reservations-api-openapi.yml
- filename: booking-com-connectivity-rates-availability-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Rates and Availability API
  slug: connectivity-rates-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-rates-availability-api-openapi.yml
- filename: booking-com-connectivity-promotions-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Promotions API
  slug: connectivity-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-promotions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Booking Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: booking-com secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: booking-com
provider_slug: booking-com
scheme_count: 3
schemes:
- description: Bearer token authentication. Include your API key token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/booking-com-car-rentals-api-openapi.yml
  - openapi/booking-com-demand-api-openapi.yml
  type: http
- description: Your Booking.com Affiliate ID, required with every request.
  in: header
  name: affiliateId
  parameter: X-Affiliate-Id
  sources:
  - openapi/booking-com-car-rentals-api-openapi.yml
  - openapi/booking-com-demand-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using your Connectivity partner username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/booking-com-connectivity-content-api-openapi.yml
  - openapi/booking-com-connectivity-promotions-api-openapi.yml
  - openapi/booking-com-connectivity-rates-availability-api-openapi.yml
  - openapi/booking-com-connectivity-reservations-api-openapi.yml
  type: http
slug: booking-com-authentication
source_filename: booking-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/booking-com-car-rentals-api-openapi.yml, openapi/booking-com-connectivity-content-api-openapi.yml,\n  openapi/booking-com-connectivity-promotions-api-openapi.yml, openapi/booking-com-connectivity-rates-availability-api-openapi.yml,\n  openapi/booking-com-connectivity-reservations-api-openapi.yml, openapi/booking-com-demand-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Include your API key token in the Authorization\n    header.\n  sources:\n  - openapi/booking-com-car-rentals-api-openapi.yml\n  - openapi/booking-com-demand-api-openapi.yml\n- name: affiliateId\n  type: apiKey\n  in: header\n  parameter: X-Affiliate-Id\n  description: Your Booking.com Affiliate ID, required with every request.\n  sources:\n  - openapi/booking-com-car-rentals-api-openapi.yml\n  - openapi/booking-com-demand-api-openapi.yml\n\
  - name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your Connectivity partner username and password.\n  sources:\n  - openapi/booking-com-connectivity-content-api-openapi.yml\n  - openapi/booking-com-connectivity-promotions-api-openapi.yml\n  - openapi/booking-com-connectivity-rates-availability-api-openapi.yml\n  - openapi/booking-com-connectivity-reservations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/authentication/booking-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags: []
---
