---
api_key_in: []
api_specs:
- filename: travelport-booking-api-openapi.yml
  format: yaml
  label: Travelport Booking API
  slug: travelport-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-booking-api-openapi.yml
- filename: travelport-emds-api-openapi.yml
  format: yaml
  label: Travelport EMDs API
  slug: travelport-emds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-emds-api-openapi.yml
- filename: travelport-fare-rules-api-openapi.yml
  format: yaml
  label: Travelport Fare Rules API
  slug: travelport-fare-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-fare-rules-api-openapi.yml
- filename: travelport-modifications-api-openapi.yml
  format: yaml
  label: Travelport Modifications API
  slug: travelport-modifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-modifications-api-openapi.yml
- filename: travelport-pricing-api-openapi.yml
  format: yaml
  label: Travelport Pricing API
  slug: travelport-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-pricing-api-openapi.yml
- filename: travelport-queues-api-openapi.yml
  format: yaml
  label: Travelport Queues API
  slug: travelport-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-queues-api-openapi.yml
- filename: travelport-reservations-api-openapi.yml
  format: yaml
  label: Travelport Reservations API
  slug: travelport-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-reservations-api-openapi.yml
- filename: travelport-search-api-openapi.yml
  format: yaml
  label: Travelport Search API
  slug: travelport-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-search-api-openapi.yml
- filename: travelport-seats-and-ancillaries-api-openapi.yml
  format: yaml
  label: Travelport Seats and Ancillaries API
  slug: travelport-seats-and-ancillaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-seats-and-ancillaries-api-openapi.yml
- filename: travelport-ticketing-api-openapi.yml
  format: yaml
  label: Travelport Ticketing API
  slug: travelport-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-ticketing-api-openapi.yml
- filename: travelport-workbench-api-openapi.yml
  format: yaml
  label: Travelport Workbench API
  slug: travelport-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-workbench-api-openapi.yml
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
