---
api_key_in: []
api_specs:
- filename: guesty-calendars-api-openapi.yml
  format: yaml
  label: Guesty Calendars API
  slug: guesty-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-calendars-api-openapi.yml
- filename: guesty-conversations-api-openapi.yml
  format: yaml
  label: Guesty Conversations API
  slug: guesty-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-conversations-api-openapi.yml
- filename: guesty-guests-api-openapi.yml
  format: yaml
  label: Guesty Guests API
  slug: guesty-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-guests-api-openapi.yml
- filename: guesty-listings-api-openapi.yml
  format: yaml
  label: Guesty Listings API
  slug: guesty-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-listings-api-openapi.yml
- filename: guesty-reservations-api-openapi.yml
  format: yaml
  label: Guesty Reservations API
  slug: guesty-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-reservations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Guesty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guesty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Guesty
provider_slug: guesty
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/guesty-openapi.yml
  type: http
slug: guesty-authentication
source_filename: guesty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guesty-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/guesty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/authentication/guesty-authentication.yml
summary_line: http · 1 scheme
tags:
- Booking
- Hospitality
- Property Management
- Reservations
- Short-Term Rentals
- Vacation Rentals
---
