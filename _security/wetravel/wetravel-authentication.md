---
api_key_in:
- header
api_specs:
- filename: wetravel-partner-openapi.json
  format: json
  label: WeTravel Partner API
  slug: wetravel-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-partner-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wetravel Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeTravel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WeTravel
provider_slug: wetravel
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wetravel-partner-openapi.json
  type: http
- in: header
  name: tokenAuth
  parameter: X-Api-Key
  sources:
  - openapi/wetravel-partner-openapi.json
  type: apiKey
slug: wetravel-authentication
source_filename: wetravel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wetravel-partner-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wetravel-partner-openapi.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/wetravel-partner-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/authentication/wetravel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Business Applications
- Travel
- Booking
- Payments
- Trip Management
- Tour Operators
- Travel Technology
---
