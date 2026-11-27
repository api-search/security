---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: orboni-com-checkout-sessions-api-openapi.yml
  format: yaml
  label: Orboni Checkout Sessions API
  slug: orboni-com-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-checkout-sessions-api-openapi.yml
- filename: orboni-com-currencies-api-openapi.yml
  format: yaml
  label: Orboni Currencies API
  slug: orboni-com-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-currencies-api-openapi.yml
- filename: orboni-com-events-api-openapi.yml
  format: yaml
  label: Orboni Events API
  slug: orboni-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-events-api-openapi.yml
- filename: orboni-com-payment-links-api-openapi.yml
  format: yaml
  label: Orboni Payment Links API
  slug: orboni-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-payment-links-api-openapi.yml
- filename: orboni-com-payment-methods-api-openapi.yml
  format: yaml
  label: Orboni Payment Methods API
  slug: orboni-com-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-payment-methods-api-openapi.yml
- filename: orboni-com-refunds-api-openapi.yml
  format: yaml
  label: Orboni Refunds API
  slug: orboni-com-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-refunds-api-openapi.yml
- filename: orboni-com-webhooks-api-openapi.yml
  format: yaml
  label: Orboni Webhooks API
  slug: orboni-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orboni-com/openapi/orboni-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Orboni Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orboni secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orboni
provider_slug: orboni-com
scheme_count: 3
schemes:
- bearerFormat: sk_live_… or sk_test_…
  description: 'Your secret key as a bearer token: `Authorization: Bearer sk_live_…`. A key’s prefix is its mode: `sk_test_…` keys make and see only test objects (`cs_test_…`, test events, test refunds), `sk_live_…` keys only live ones; the two never meet. Keys are per project and per mode, made and revoked in the dashboard under Developers → API keys, shown once. Keep a secret key on your server, never in a brow'
  name: secretKey
  scheme: bearer
  sources:
  - openapi/orboni-com-openapi.yml
  type: http
- description: 'The same secret key as the user of HTTP basic auth with an empty password (`curl -u sk_live_…:`), as Stripe’s client libraries send it. A key’s prefix is its mode: `sk_test_…` keys make and see only test objects (`cs_test_…`, test events, test refunds), `sk_live_…` keys only live ones; the two never meet. Keys are per project and per mode, made and revoked in the dashboard under Developers → API k'
  name: secretKeyBasic
  scheme: basic
  sources:
  - openapi/orboni-com-openapi.yml
  type: http
- description: 'The project’s publishable key, `pk_live_…` or `pk_test_…` (Developers → API keys). Safe on a public page: it is good only for `GET /public/payment_methods` and makes, reads or changes nothing else. Its prefix is its mode.'
  in: query
  name: publishableKey
  parameter: key
  sources:
  - openapi/orboni-com-openapi.yml
  type: apiKey
slug: orboni-com-authentication
source_filename: orboni-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/orboni-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: secretKey\n  type: http\n  scheme: bearer\n  bearerFormat: sk_live_… or sk_test_…\n  description: 'Your secret key as a bearer token: `Authorization: Bearer sk_live_…`. A key’s\n    prefix is its mode: `sk_test_…` keys make and see only test objects (`cs_test_…`, test events,\n    test refunds), `sk_live_…` keys only live ones; the two never meet. Keys are per project\n    and per mode, made and revoked in the dashboard under Developers → API keys, shown once.\n    Keep a secret key on your server, never in a brow'\n  sources:\n  - openapi/orboni-com-openapi.yml\n- name: secretKeyBasic\n  type: http\n  scheme: basic\n  description: 'The same secret key as the user of HTTP basic auth with an empty password (`curl\n    -u sk_live_…:`), as Stripe’s client libraries send it. A key’s prefix is its mode: `sk_test_…`\n\
  \    keys make and see only test objects (`cs_test_…`, test events, test refunds), `sk_live_…`\n    keys only live ones; the two never meet. Keys are per project and per mode, made and revoked\n    in the dashboard under Developers → API k'\n  sources:\n  - openapi/orboni-com-openapi.yml\n- name: publishableKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: 'The project’s publishable key, `pk_live_…` or `pk_test_…` (Developers → API\n    keys). Safe on a public page: it is good only for `GET /public/payment_methods` and makes,\n    reads or changes nothing else. Its prefix is its mode.'\n  sources:\n  - openapi/orboni-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/orboni-com/authentication/orboni-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Checkout
- Crypto Payments
- Non-Custodial
- Online Payments
- Payment Gateway
- Webhook
---
