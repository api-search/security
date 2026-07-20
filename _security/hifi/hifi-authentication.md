---
api_key_in:
- header
api_specs:
- filename: hifi-openapi-original.json
  format: json
  label: Hifi API
  slug: hifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hifi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hifi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hifi
provider_slug: hifi
scheme_count: 1
schemes:
- bearerFormat: JWT
  header_name: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hifi-openapi-original.json
  type: http
slug: hifi-authentication
source_filename: hifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hifi-openapi-original.json\ndocs: https://docs.hifi.com/api/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  scheme: All requests are authenticated with a bearer API key sent in the\n    Authorization header over HTTPS/TLS. Keys are created in the Hifi Dashboard\n    under Developer > API Keys and shown only once at creation.\nnotes:\n- Header format is \"Authorization: Bearer [example key]\".\n- Separate keys per environment; sandbox keys must never be used in production\n  and vice versa. There is no documented test/live key prefix.\n- Webhook callbacks are themselves signed as an RS256 JWT in the Authorization\n  header, verified with the per-endpoint webhook public key.\n- Recommended rotation is annual, or immediately on suspected compromise.\nenvironments:\n- name: sandbox\n  base_url: https://sandbox.hifibridge.com\n- name: production\n  base_url: https://production.hifibridge.com\n\
  schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header_name: Authorization\n  sources:\n  - openapi/hifi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/authentication/hifi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Stablecoins
- Payments
- Money Movement
- On-Ramp
- Off-Ramp
- Crypto
- Fintech
- KYC
- Virtual Accounts
- Cross-Chain
- Financial Infrastructure
---
