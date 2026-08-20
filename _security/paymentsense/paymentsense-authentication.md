---
api_key_in:
- header
api_specs:
- filename: paymentsense-connect-v2.json
  format: json
  label: Paymentsense Connect REST API
  slug: connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-connect-v2.json
- filename: paymentsense-connect-e-v0.json
  format: json
  label: Paymentsense Connect-E REST API
  slug: connect-e-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-connect-e-v0.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paymentsense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paymentsense secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paymentsense
provider_slug: paymentsense
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/paymentsense-connect-e-v0.json
  type: apiKey
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/paymentsense-connect-e-v0.json
  type: http
- name: connectBasicAuth
  scheme: basic
  sources:
  - openapi/paymentsense-connect-v0.json
  - openapi/paymentsense-connect-v1.json
  - openapi/paymentsense-connect-v2.json
  type: http
slug: paymentsense-authentication
source_filename: paymentsense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/paymentsense-connect-e-v0.json, openapi/paymentsense-connect-v0.json, openapi/paymentsense-connect-v1.json,\n  openapi/paymentsense-connect-v2.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/paymentsense-connect-e-v0.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/paymentsense-connect-e-v0.json\n- name: connectBasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/paymentsense-connect-v0.json\n  - openapi/paymentsense-connect-v1.json\n  - openapi/paymentsense-connect-v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/authentication/paymentsense-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Card Payments
- Acquiring
- Point-of-Sale
- In-Person Payments
---
