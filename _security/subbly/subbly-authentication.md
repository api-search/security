---
api_key_in:
- header
api_specs:
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Products API
  slug: subbly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Subscriptions API
  slug: subbly-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Customers API
  slug: subbly-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Cart and Checkout API
  slug: subbly-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Subbly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Subbly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Subbly
provider_slug: subbly
scheme_count: 1
schemes:
- description: Modeled. Subbly's storefront SDK is configured with an apiKey issued in the Subbly admin (Shop Settings). The exact header/parameter name is not published by Subbly.
  in: header
  name: apiKey
  parameter: X-Subbly-Api-Key
  sources:
  - openapi/subbly-openapi.yml
  type: apiKey
slug: subbly-authentication
source_filename: subbly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/subbly-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Subbly-Api-Key\n  description: Modeled. Subbly's storefront SDK is configured with an apiKey issued in the Subbly\n    admin (Shop Settings). The exact header/parameter name is not published by Subbly.\n  sources:\n  - openapi/subbly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/authentication/subbly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscriptions
- Subscription Commerce
- Ecommerce
- Subscription Box
- Recurring Billing
- Headless Commerce
- SDK
- Webhooks
---
