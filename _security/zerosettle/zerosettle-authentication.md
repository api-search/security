---
api_key_in:
- header
api_specs:
- filename: zerosettle-cancel-flow-api-openapi.yml
  format: yaml
  label: ZeroSettle Cancel Flow API
  slug: zerosettle-cancel-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-cancel-flow-api-openapi.yml
- filename: zerosettle-checkout-api-openapi.yml
  format: yaml
  label: ZeroSettle Checkout API
  slug: zerosettle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-checkout-api-openapi.yml
- filename: zerosettle-entitlements-api-openapi.yml
  format: yaml
  label: ZeroSettle Entitlements API
  slug: zerosettle-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-entitlements-api-openapi.yml
- filename: zerosettle-events-api-openapi.yml
  format: yaml
  label: ZeroSettle Events API
  slug: zerosettle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-events-api-openapi.yml
- filename: zerosettle-migration-api-openapi.yml
  format: yaml
  label: ZeroSettle Migration API
  slug: zerosettle-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-migration-api-openapi.yml
- filename: zerosettle-products-api-openapi.yml
  format: yaml
  label: ZeroSettle Products API
  slug: zerosettle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-products-api-openapi.yml
- filename: zerosettle-restore-api-openapi.yml
  format: yaml
  label: ZeroSettle Restore API
  slug: zerosettle-restore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-restore-api-openapi.yml
- filename: zerosettle-storekit-api-openapi.yml
  format: yaml
  label: ZeroSettle StoreKit API
  slug: zerosettle-storekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-storekit-api-openapi.yml
- filename: zerosettle-subscriptions-api-openapi.yml
  format: yaml
  label: ZeroSettle Subscriptions API
  slug: zerosettle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-subscriptions-api-openapi.yml
- filename: zerosettle-transactions-api-openapi.yml
  format: yaml
  label: ZeroSettle Transactions API
  slug: zerosettle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-transactions-api-openapi.yml
- filename: zerosettle-upgrade-offers-api-openapi.yml
  format: yaml
  label: ZeroSettle Upgrade Offers API
  slug: zerosettle-upgrade-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-upgrade-offers-api-openapi.yml
- filename: zerosettle-user-offer-api-openapi.yml
  format: yaml
  label: ZeroSettle User Offer API
  slug: zerosettle-user-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-user-offer-api-openapi.yml
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
- Subscription
- Merchant of Record
- Billing
- Mobile
- Developer Tools
---
