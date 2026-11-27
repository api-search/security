---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tickets-dev-capture-api-openapi.yml
  format: yaml
  label: Tickets.dev Capture API
  slug: tickets-dev-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-capture-api-openapi.yml
- filename: tickets-dev-events-api-openapi.yml
  format: yaml
  label: Tickets.dev Events API
  slug: tickets-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-events-api-openapi.yml
- filename: tickets-dev-health-api-openapi.yml
  format: yaml
  label: Tickets.dev Health API
  slug: tickets-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickets-dev/openapi/tickets-dev-health-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tickets.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tickets.dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tickets.dev
provider_slug: tickets-dev
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/tickets-dev-openapi.json
  type: apiKey
slug: tickets-dev-authentication
source_filename: tickets-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/tickets-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/tickets-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tickets-dev/authentication/tickets-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ticketing
- Market Data
- Pricing
- Inventory
- Seat Maps
- Resale
- Event
---
