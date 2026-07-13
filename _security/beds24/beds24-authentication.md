---
api_key_in:
- header
api_specs:
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Authentication API
  slug: beds24-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Bookings API
  slug: beds24-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Invoices & Charges API
  slug: beds24-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Booking Messages API
  slug: beds24-booking-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Properties API
  slug: beds24-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Availability & Calendar API
  slug: beds24-availability-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Rates & Prices API
  slug: beds24-rates-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Channels API
  slug: beds24-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Accounts API
  slug: beds24-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Beds24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beds24 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beds24
provider_slug: beds24
scheme_count: 1
schemes:
- description: Short-lived access token generated from a refresh token via the /authentication endpoints, sent in the "token" request header.
  in: header
  name: tokenAuth
  parameter: token
  sources:
  - openapi/beds24-openapi.yml
  type: apiKey
slug: beds24-authentication
source_filename: beds24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beds24-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: token\n  description: Short-lived access token generated from a refresh token via the /authentication\n    endpoints, sent in the \"token\" request header.\n  sources:\n  - openapi/beds24-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/authentication/beds24-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vacation Rental
- Hotel
- Channel Manager
- Property Management System
- Booking Engine
- Hospitality
- Reservations
---
