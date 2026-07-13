---
api_key_in: []
api_specs:
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Products & Variants API
  slug: products-variants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy License Keys API
  slug: license-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Discounts API
  slug: discounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemonsqueezy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemon Squeezy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemon Squeezy
provider_slug: lemonsqueezy
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: Bearer authentication using a Lemon Squeezy API key. Requests must also send Accept and Content-Type headers of application/vnd.api+json.
  name: api_key
  scheme: bearer
  sources:
  - openapi/lemonsqueezy-openapi.yml
  type: http
slug: lemonsqueezy-authentication
source_filename: lemonsqueezy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lemonsqueezy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: Bearer authentication using a Lemon Squeezy API key. Requests must also send\n    Accept and Content-Type headers of application/vnd.api+json.\n  sources:\n  - openapi/lemonsqueezy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/authentication/lemonsqueezy-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Merchant of Record
- Subscriptions
- Digital Products
- SaaS
- Sales Tax
---
