---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: inboxpolicy-com-verification-api-openapi.yml
  format: yaml
  label: inboxpolicy-com Verification API
  slug: inboxpolicy-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxpolicy-com/openapi/inboxpolicy-com-verification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Inboxpolicy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: inboxpolicy-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: inboxpolicy-com
provider_slug: inboxpolicy-com
scheme_count: 1
schemes:
- description: x402 v2 payment signature header for paid operations.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/inboxpolicy-com-openapi.json
  type: apiKey
slug: inboxpolicy-com-authentication
source_filename: inboxpolicy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/inboxpolicy-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 payment signature header for paid operations.\n  sources:\n  - openapi/inboxpolicy-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/inboxpolicy-com/authentication/inboxpolicy-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- EmailVerification
- API
- AI
- Payments
- Pricing
---
