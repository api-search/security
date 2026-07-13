---
api_key_in: []
api_specs:
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Products & Prices API
  slug: products-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Benefits & License Keys API
  slug: benefits-license-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Meters & Events API
  slug: meters-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polar Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polar
provider_slug: polar-sh
scheme_count: 1
schemes:
- description: Organization Access Token used for backend, organization-scoped operations.
  name: oat
  scheme: bearer
  sources:
  - openapi/polar-sh-openapi.yml
  type: http
slug: polar-sh-authentication
source_filename: polar-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polar-sh-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oat\n  type: http\n  scheme: bearer\n  description: Organization Access Token used for backend, organization-scoped operations.\n  sources:\n  - openapi/polar-sh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/authentication/polar-sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Payments
- Merchant of Record
- Monetization
- Subscriptions
- Usage Based Billing
---
