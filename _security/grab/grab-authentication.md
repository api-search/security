---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Grab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grab
provider_slug: grab
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/grab-openapi.yml
  type: http
slug: grab-authentication
source_filename: grab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grab-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/grab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grab/refs/heads/main/authentication/grab-authentication.yml
summary_line: http · 1 scheme
tags:
- Ride Hailing
- Food Delivery
- Last-Mile Logistics
- Digital Payments
- Superapp
- Southeast Asia
- Identity
- Loyalty
- QR Payments
- OAuth2
---
