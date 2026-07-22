---
api_key_in:
- header
api_specs:
- filename: tabapay-openapi.yml
  format: yaml
  label: TabaPay Unified API
  slug: tabapay-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tabapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: TabaPay secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TabaPay
provider_slug: tabapay
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tabapay-openapi.yml
  type: http
- in: header
  name: custom-header
  parameter: Authorization
  sources:
  - openapi/tabapay-openapi.yml
  type: apiKey
slug: tabapay-authentication
source_filename: tabapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tabapay-openapi.yml + https://developers.tabapay.com/reference/getting-started\ndocs: https://developers.tabapay.com/reference/getting-started\nnotes: TabaPay APIs are not publicly self-serve — a static bearer access token (API key) is\n  issued at boarding along with a client-specific FQDN, and requests must come from allowlisted\n  IPs (sandbox and production IPs must differ). Expired sandbox credentials are renewed via\n  help@tabapay.com. Card data may additionally be RSA-encrypted client-side using keys managed\n  through the Key API (keyCreate/keyRetrieve/keyDelete).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tabapay-openapi.yml\n- name: custom-header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/tabapay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/authentication/tabapay-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Payments
- Instant Payments
- Money Movement
- Payouts
- Cards
- Real-Time Payments
- ACH
---
