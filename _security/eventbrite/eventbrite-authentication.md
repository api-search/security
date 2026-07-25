---
api_key_in: []
api_specs:
- filename: eventbrite-attendees-api-openapi.yml
  format: yaml
  label: Eventbrite Attendees API
  slug: eventbrite-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-attendees-api-openapi.yml
- filename: eventbrite-categories-api-openapi.yml
  format: yaml
  label: Eventbrite Categories API
  slug: eventbrite-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-categories-api-openapi.yml
- filename: eventbrite-events-api-openapi.yml
  format: yaml
  label: Eventbrite Events API
  slug: eventbrite-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-events-api-openapi.yml
- filename: eventbrite-orders-api-openapi.yml
  format: yaml
  label: Eventbrite Orders API
  slug: eventbrite-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-orders-api-openapi.yml
- filename: eventbrite-organizations-api-openapi.yml
  format: yaml
  label: Eventbrite Organizations API
  slug: eventbrite-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-organizations-api-openapi.yml
- filename: eventbrite-ticket-classes-api-openapi.yml
  format: yaml
  label: Eventbrite Ticket Classes API
  slug: eventbrite-ticket-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-ticket-classes-api-openapi.yml
- filename: eventbrite-users-api-openapi.yml
  format: yaml
  label: Eventbrite Users API
  slug: eventbrite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-users-api-openapi.yml
- filename: eventbrite-venues-api-openapi.yml
  format: yaml
  label: Eventbrite Venues API
  slug: eventbrite-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-venues-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eventbrite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eventbrite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eventbrite
provider_slug: eventbrite
scheme_count: 1
schemes:
- description: OAuth 2.0 token (private token or OAuth-issued)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eventbrite-openapi.yml
  type: http
slug: eventbrite-authentication
source_filename: eventbrite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eventbrite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 token (private token or OAuth-issued)\n  sources:\n  - openapi/eventbrite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/authentication/eventbrite-authentication.yml
summary_line: http · 1 scheme
tags:
- Events
- Event Technology
- Ticketing
- Marketplace
---
