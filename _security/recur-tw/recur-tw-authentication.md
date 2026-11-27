---
anonymous_access: false
api_key_in: []
api_specs:
- filename: recur-tw-checkout-sessions-api-openapi.yml
  format: yaml
  label: Recur Checkout Sessions API
  slug: recur-tw-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-checkout-sessions-api-openapi.yml
- filename: recur-tw-products-api-openapi.yml
  format: yaml
  label: Recur Products API
  slug: recur-tw-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-products-api-openapi.yml
- filename: recur-tw-subscription-schedules-api-openapi.yml
  format: yaml
  label: Recur Subscription Schedules API
  slug: recur-tw-subscription-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-schedules-api-openapi.yml
- filename: recur-tw-subscription-switching-api-openapi.yml
  format: yaml
  label: Recur Subscription Switching API
  slug: recur-tw-subscription-switching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-switching-api-openapi.yml
- filename: recur-tw-subscriptions-api-openapi.yml
  format: yaml
  label: Recur Subscriptions API
  slug: recur-tw-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Recur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recur declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Recur
provider_slug: recur-tw
scheme_count: 2
schemes:
- evidence: '# Secret Key curl https://api.recur.tw/v1/checkout/sessions \ -H "X-Recur-Secret-Key: sk_test_xxx"'
  header: X-Recur-Secret-Key
  how_to_obtain: Provide Secret Key in X-Recur-Secret-Key header
  location: header
  name: X-Recur-Secret-Key Header
  type: apiKey
- evidence: '# Publishable Key curl https://api.recur.tw/v1/products \ -H "X-Recur-Publishable-Key: pk_test_xxx"'
  header: X-Recur-Publishable-Key
  how_to_obtain: Provide Publishable Key in X-Recur-Publishable-Key header
  location: header
  name: X-Recur-Publishable-Key Header
  type: apiKey
slug: recur-tw-authentication
source_filename: recur-tw-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.recur.tw/getting-started/authentication
source_yaml: "generated: '2026-11-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.recur.tw/getting-started/authentication\nsources:\n- https://docs.recur.tw/getting-started/authentication\n- https://docs.recur.tw/getting-started\n- https://docs.recur.tw/getting-started/quick-start\n- https://docs.recur.tw/getting-started/sdk\nschemes:\n- type: apiKey\n  name: X-Recur-Secret-Key Header\n  evidence: '# Secret Key curl https://api.recur.tw/v1/checkout/sessions \\ -H \"X-Recur-Secret-Key: sk_test_xxx\"'\n  location: header\n  header: X-Recur-Secret-Key\n  how_to_obtain: Provide Secret Key in X-Recur-Secret-Key header\n- type: apiKey\n  name: X-Recur-Publishable-Key Header\n  evidence: '# Publishable Key curl https://api.recur.tw/v1/products \\ -H \"X-Recur-Publishable-Key: pk_test_xxx\"'\n  location: header\n  header: X-Recur-Publishable-Key\n  how_to_obtain: Provide Publishable Key in X-Recur-Publishable-Key header\ndocs: https://docs.recur.tw/getting-started/authentication\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/recur-tw/authentication/recur-tw-authentication.yml
summary_line: 2 schemes
tags:
- Subscription
- Payments
- CreatorEconomy
- Taiwan
- SaaS
---
