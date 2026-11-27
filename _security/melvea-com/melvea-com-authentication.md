---
anonymous_access: false
api_key_in: []
api_specs:
- filename: melvea-com-free-api-openapi.yml
  format: yaml
  label: Melvea Free API
  slug: melvea-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/melvea-com/openapi/melvea-com-free-api-openapi.yml
- filename: melvea-com-x402-api-openapi.yml
  format: yaml
  label: Melvea X402 API
  slug: melvea-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/melvea-com/openapi/melvea-com-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Melvea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Melvea secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Melvea
provider_slug: melvea-com
scheme_count: 1
schemes:
- description: x402 payment. Unpaid requests receive HTTP 402 with a base64 payment-required header; resubmit with X-PAYMENT / payment-signature.
  name: x402
  scheme: bearer
  sources:
  - openapi/melvea-com-openapi.json
  type: http
slug: melvea-com-authentication
source_filename: melvea-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/melvea-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: x402\n  type: http\n  scheme: bearer\n  description: x402 payment. Unpaid requests receive HTTP 402 with a base64 payment-required\n    header; resubmit with X-PAYMENT / payment-signature.\n  sources:\n  - openapi/melvea-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/melvea-com/authentication/melvea-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Honey
- Food
- Media
- Data
- Consumer
---
