---
api_key_in: []
api_specs:
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Partner API
  slug: eat-app-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Reservations API
  slug: eat-app-concierge-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Guests API
  slug: eat-app-concierge-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Availability API
  slug: eat-app-concierge-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Restaurants and Groups API
  slug: eat-app-concierge-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Tables and Floorplan API
  slug: eat-app-tables-floorplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eat App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eat App secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eat App
provider_slug: eat-app
scheme_count: 1
schemes:
- description: 'Bearer token (the API key Eat App issues to a partner or Concierge user). Sent as Authorization: Bearer <api_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eat-app-openapi.yml
  type: http
slug: eat-app-authentication
source_filename: eat-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eat-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token (the API key Eat App issues to a partner or Concierge user). Sent\n    as Authorization: Bearer <api_token>.'\n  sources:\n  - openapi/eat-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/authentication/eat-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Restaurant
- Reservations
- Table Management
- Hospitality
- Bookings
- Guest CRM
- Availability
---
