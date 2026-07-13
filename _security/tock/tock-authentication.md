---
api_key_in:
- header
api_specs:
- filename: tock-reservation-openapi.yml
  format: yaml
  label: Tock Reservation API
  slug: reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/openapi/tock-reservation-openapi.yml
- filename: tock-guest-profile-openapi.yml
  format: yaml
  label: Tock Guest API
  slug: guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/openapi/tock-guest-profile-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tock secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tock
provider_slug: tock
scheme_count: 1
schemes:
- description: Tock-issued API key. Request access by emailing integrate@tockhq.com from a Tock Dashboard Account Owner; available on Premium and Premium Unlimited plans.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tock-guest-profile-openapi.yml
  - openapi/tock-reservation-openapi.yml
  type: apiKey
slug: tock-authentication
source_filename: tock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tock-guest-profile-openapi.yml, openapi/tock-reservation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Tock-issued API key. Request access by emailing integrate@tockhq.com from a Tock\n    Dashboard Account Owner; available on Premium and Premium Unlimited plans.\n  sources:\n  - openapi/tock-guest-profile-openapi.yml\n  - openapi/tock-reservation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/authentication/tock-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Reservations
- Restaurants
- Wineries
- Ticketed Events
- Takeout
- Delivery
- Experiences
- Dining
- American Express
---
