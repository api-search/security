---
api_key_in:
- header
api_specs:
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Rates & Availability API
  slug: rates-availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Bookings & Reservations API
  slug: bookings-reservations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lodgify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lodgify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lodgify
provider_slug: lodgify
scheme_count: 1
schemes:
- description: Account API key passed in the X-ApiKey request header.
  in: header
  name: ApiKeyAuth
  parameter: X-ApiKey
  sources:
  - openapi/lodgify-openapi.yml
  type: apiKey
slug: lodgify-authentication
source_filename: lodgify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lodgify-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ApiKey\n  description: Account API key passed in the X-ApiKey request header.\n  sources:\n  - openapi/lodgify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/authentication/lodgify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vacation Rental
- Property Management
- Booking
- Channel Manager
- Travel
---
