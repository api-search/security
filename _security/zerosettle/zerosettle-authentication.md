---
api_key_in:
- header
api_specs:
- filename: zerosettle-openapi.json
  format: json
  label: ZeroSettle IAP API
  slug: zerosettle-iap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zerosettle Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZeroSettle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZeroSettle
provider_slug: zerosettle
scheme_count: 1
schemes:
- description: Your publishable API key. Use `zs_pk_test_*` for sandbox or `zs_pk_live_*` for production.
  in: header
  name: ApiKeyAuth
  parameter: X-ZeroSettle-Key
  sources:
  - openapi/zerosettle-openapi.json
  type: apiKey
slug: zerosettle-authentication
source_filename: zerosettle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zerosettle-openapi.json\ndocs: https://docs.zerosettle.io/iap/account-setup\nnotes: >-\n  Single publishable API key sent in the X-ZeroSettle-Key header. The key prefix\n  selects the environment — zs_pk_test_* for sandbox (Stripe test), zs_pk_live_*\n  for live. No OAuth2/OIDC on the API surface (Stripe Connect OAuth is a\n  dashboard/BYOS onboarding concern, not an API auth scheme).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ZeroSettle-Key\n  description: Your publishable API key. Use `zs_pk_test_*` for sandbox or `zs_pk_live_*` for\n    production.\n  sources:\n  - openapi/zerosettle-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/authentication/zerosettle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- In-App Purchase
- Subscriptions
- Merchant of Record
- Billing
- Mobile
- Developer Tools
---
