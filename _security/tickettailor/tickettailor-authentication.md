---
api_key_in: []
api_specs:
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Events API
  slug: tickettailor-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Event Series API
  slug: tickettailor-event-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Orders API
  slug: tickettailor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Issued Tickets API
  slug: tickettailor-issued-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Vouchers API
  slug: tickettailor-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Check-ins API
  slug: tickettailor-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tickettailor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ticket Tailor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ticket Tailor
provider_slug: tickettailor
scheme_count: 1
schemes:
- description: HTTP Basic Auth. Supply your Ticket Tailor API key as the username and leave the password blank. Keys are managed in box office settings and are scoped to the issuing box office.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tickettailor-openapi.yml
  type: http
slug: tickettailor-authentication
source_filename: tickettailor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tickettailor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Supply your Ticket Tailor API key as the username and leave\n    the password blank. Keys are managed in box office settings and are scoped to the issuing\n    box office.\n  sources:\n  - openapi/tickettailor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/authentication/tickettailor-authentication.yml
summary_line: http · 1 scheme
tags:
- Event Ticketing
- Events
- Ticketing
- Box Office
- Payments
- Registration
---
