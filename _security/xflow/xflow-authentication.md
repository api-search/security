---
api_key_in: []
api_specs:
- filename: xflow-openapi-original.yml
  format: yaml
  label: Xflow API
  slug: xflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Xflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xflow
provider_slug: xflow
scheme_count: 1
schemes:
- bearerFormat: auth-scheme
  description: 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xflow-openapi-original.yml
  type: http
slug: xflow-authentication
source_filename: xflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/xflow-openapi-original.yml\ndocs: https://docs.xflowpay.com/latest/api\nsummary:\n  types:\n  - http\n  styles:\n  - bearer\n  - basic (API key as username, empty password)\n  key_prefixes:\n    test: sk_test_\n    live: sk_live_\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: auth-scheme\n  description: 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'\n  sources:\n  - openapi/xflow-openapi-original.yml\nnotes: API keys are managed in the Xflow dashboard. Test keys are prefixed sk_test_\n  and live keys sk_live_; testmode and livemode data are fully separate. The docs\n  also allow supplying the API key as the HTTP Basic auth username with no\n  password. All requests must use HTTPS; plain HTTP calls fail. Platforms act on\n  behalf of connected users with the Xflow-Account header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/authentication/xflow-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cross-Border Payments
- Fintech
- India
- Foreign Exchange
- Invoicing
- Payouts
---
