---
api_key_in: []
api_specs:
- filename: launch27-account-api-openapi.yml
  format: yaml
  label: Launch27 Account API
  slug: launch27-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-account-api-openapi.yml
- filename: launch27-authentication-api-openapi.yml
  format: yaml
  label: Launch27 Authentication API
  slug: launch27-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-authentication-api-openapi.yml
- filename: launch27-booking-helpers-api-openapi.yml
  format: yaml
  label: Launch27 Booking Helpers API
  slug: launch27-booking-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-booking-helpers-api-openapi.yml
- filename: launch27-customer-bookings-api-openapi.yml
  format: yaml
  label: Launch27 Customer Bookings API
  slug: launch27-customer-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-customer-bookings-api-openapi.yml
- filename: launch27-guest-booking-api-openapi.yml
  format: yaml
  label: Launch27 Guest Booking API
  slug: launch27-guest-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-guest-booking-api-openapi.yml
- filename: launch27-policy-api-openapi.yml
  format: yaml
  label: Launch27 Policy API
  slug: launch27-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-policy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Launch27 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Launch27 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Launch27
provider_slug: launch27
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT returned as `bearer` in the Login response. Sent as `Authorization: Bearer <JWT>`. A legacy `email:token` form (Authorization: email:token) existed but was retired March 1, 2023.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/launch27-openapi.yml
  type: http
slug: launch27-authentication
source_filename: launch27-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/launch27-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT returned as `bearer` in the Login response. Sent as `Authorization: Bearer\n    <JWT>`. A legacy `email:token` form (Authorization: email:token) existed but was retired\n    March 1, 2023.'\n  sources:\n  - openapi/launch27-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/authentication/launch27-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Home Services
- Cleaning Services
- Booking
- Scheduling
- Fullsteam
- Vonigo
---
