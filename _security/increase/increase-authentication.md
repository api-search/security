---
api_key_in: []
api_specs:
- filename: increase-openapi.json
  format: json
  label: Increase ACH API
  slug: increase-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Wire Transfers API
  slug: increase-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Real-Time Payments API
  slug: increase-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Check API
  slug: increase-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Cards API
  slug: increase-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Accounts API
  slug: increase-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Increase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Increase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Increase
provider_slug: increase
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/increase-openapi.json
  type: http
slug: increase-authentication
source_filename: increase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/increase-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/increase-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/authentication/increase-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Banking
- Payments
- ACH
- Wires
---
