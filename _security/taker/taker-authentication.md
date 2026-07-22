---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Taker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taker
provider_slug: taker
scheme_count: 1
schemes:
- format: Bearer <TOKEN>
  in: header
  name: bearerAuth
  parameter: Authorization
  required_headers:
  - 'Authorization: Bearer <TOKEN>'
  - 'Content-Type: application/json'
  roles:
  - name: TAKERGO_TOKEN
    used_by: Restaurant integration (Taker GO merchant)
  - name: DSP_TOKEN
    used_by: Delivery Service Provider integration
  scheme: bearer
  sources:
  - https://api.help.taker.io/
  type: http
slug: taker-authentication
source_filename: taker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.help.taker.io/\ndocs: https://api.help.taker.io/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  token_delivery: Authorization header\n  notes: >-\n    The Taker GO integration API uses static bearer tokens issued by Taker. Two\n    distinct token roles exist: TAKERGO_TOKEN for restaurant-side integrations\n    and DSP_TOKEN for delivery-service-provider (DSP) integrations. There is no\n    OAuth, OpenID Connect, or scope surface documented.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Bearer <TOKEN>\"\n    roles:\n      - name: TAKERGO_TOKEN\n        used_by: Restaurant integration (Taker GO merchant)\n      - name: DSP_TOKEN\n        used_by: Delivery Service Provider integration\n    required_headers:\n      - \"Authorization: Bearer <TOKEN>\"\n      - \"Content-Type: application/json\"\n    sources: [https://api.help.taker.io/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taker/refs/heads/main/authentication/taker-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Restaurant Technology
- Online Ordering
- Food Delivery
- Delivery Integration
- Webhooks
- Saudi Arabia
- MENA
---
