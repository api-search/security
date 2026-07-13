---
api_key_in: []
api_specs:
- filename: fedex-openapi.yml
  format: yaml
  label: FedEx Track API
  slug: track
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fedex/refs/heads/main/openapi/fedex-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fedex Authentication
name_suffix: Authentication
oauth_flows: []
overview: FedEx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FedEx
provider_slug: fedex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 access token returned by POST /oauth/token using

    client_credentials with FedEx Developer Portal credentials.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fedex-openapi.yml
  type: http
slug: fedex-authentication
source_filename: fedex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fedex-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token returned by POST /oauth/token using\n    client_credentials with FedEx Developer Portal credentials.\n  sources:\n  - openapi/fedex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fedex/refs/heads/main/authentication/fedex-authentication.yml
summary_line: http · 1 scheme
tags:
- Address Validation
- Freight
- Logistics
- Pickup
- Rating
- Shipping
- Tracking
- Webhooks
- Fortune 100
---
