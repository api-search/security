---
api_key_in: []
api_specs:
- filename: microsoft-bookings-openapi.yml
  format: yaml
  label: Microsoft Graph Bookings API
  slug: graph-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Bookings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bookings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Bookings
provider_slug: microsoft-bookings
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-bookings-openapi.yml
  type: http
slug: microsoft-bookings-authentication
source_filename: microsoft-bookings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bookings-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-bookings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/authentication/microsoft-bookings-authentication.yml
summary_line: http · 1 scheme
tags:
- Bookings
- Scheduling
- Appointments
- Microsoft Graph
---
