---
api_key_in:
- header
api_specs:
- filename: sheeva-openapi.yml
  format: yaml
  label: SheevaConnect API
  slug: sheevaconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sheeva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sheeva secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sheeva
provider_slug: sheeva
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Access token obtained from GET /v2/auth (exchange client-id/client-secret), sent in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sheeva-openapi.yml
  type: http
- description: client-id + client-secret headers on GET /v2/auth to obtain an access token.
  in: header
  name: clientCredentials
  parameter: client-id
  sources:
  - openapi/sheeva-openapi.yml
  type: apiKey
slug: sheeva-authentication
source_filename: sheeva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sheeva-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token obtained from GET /v2/auth (exchange client-id/client-secret), sent\n    in the Authorization header.\n  sources:\n  - openapi/sheeva-openapi.yml\n- name: clientCredentials\n  type: apiKey\n  in: header\n  parameter: client-id\n  description: client-id + client-secret headers on GET /v2/auth to obtain an access token.\n  sources:\n  - openapi/sheeva-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/authentication/sheeva-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Connected Vehicles
- Automotive
- Payments
- Fintech
- In-Vehicle Payments
- EV Charging
- Parking
- Location Intelligence
- Mobility
---
