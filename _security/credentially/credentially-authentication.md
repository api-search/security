---
api_key_in: []
api_specs:
- filename: credentially-gateway-openapi-original.json
  format: json
  label: Credentially Public API
  slug: credentially-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/openapi/credentially-gateway-openapi-original.json
- filename: credentially-webhook-openapi-original.json
  format: json
  label: Credentially Webhook API
  slug: credentially-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/openapi/credentially-webhook-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Credentially Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credentially secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credentially
provider_slug: credentially
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer-key
  scheme: bearer
  sources:
  - openapi/credentially-gateway-openapi-original.json
  - openapi/credentially-webhook-openapi-original.json
  type: http
slug: credentially-authentication
source_filename: credentially-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/credentially-gateway-openapi-original.json, openapi/credentially-webhook-openapi-original.json\ndocs: https://credentially.readme.io/reference/getting-started-with-your-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nnotes: >-\n  API keys are provisioned per organisation by a Credentially Customer Success Manager\n  (support@credentially.io); pass as \"Authorization: Bearer <API key>\" (JWT). Keys grant\n  access to all of the organisation's staff documents and data, so must be kept confidential.\n  Webhook callbacks use a separate per-subscription Basic auth credential set by the subscriber.\nschemes:\n- name: bearer-key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/credentially-gateway-openapi-original.json\n  - openapi/credentially-webhook-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/authentication/credentially-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Credentialing
- Compliance
- Onboarding
- Workforce
- Identity Verification
- Background Checks
- NHS
- Company
---
