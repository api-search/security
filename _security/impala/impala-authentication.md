---
api_key_in:
- header
api_specs:
- filename: impala-hotels-openapi-original.json
  format: json
  label: Impala Hotel Booking API
  slug: impala-hotel-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impala/refs/heads/main/openapi/impala-hotels-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Impala Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impala secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Impala
provider_slug: impala
scheme_count: 2
schemes:
- in: header
  name: API_Key_Authentication
  parameter: x-api-key
  sources:
  - openapi/impala-hotels-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: paymentAuth
  scheme: bearer
  sources:
  - openapi/impala-hotels-openapi-original.json
  type: http
slug: impala-authentication
source_filename: impala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/impala-hotels-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: API_Key_Authentication\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/impala-hotels-openapi-original.json\n- name: paymentAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/impala-hotels-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impala/refs/heads/main/authentication/impala-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Hotels
- Travel
- Booking
- Hospitality
- Payments
- Defunct
---
