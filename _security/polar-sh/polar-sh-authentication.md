---
anonymous_access: false
api_key_in: []
api_specs:
- filename: polar-sh-benefits-api-openapi.yml
  format: yaml
  label: Polar Benefits API
  slug: polar-sh-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-benefits-api-openapi.yml
- filename: polar-sh-checkouts-api-openapi.yml
  format: yaml
  label: Polar Checkouts API
  slug: polar-sh-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-checkouts-api-openapi.yml
- filename: polar-sh-customer-portal-api-openapi.yml
  format: yaml
  label: Polar Customer Portal API
  slug: polar-sh-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-customer-portal-api-openapi.yml
- filename: polar-sh-customers-api-openapi.yml
  format: yaml
  label: Polar Customers API
  slug: polar-sh-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-customers-api-openapi.yml
- filename: polar-sh-events-api-openapi.yml
  format: yaml
  label: Polar Events API
  slug: polar-sh-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-events-api-openapi.yml
- filename: polar-sh-license-keys-api-openapi.yml
  format: yaml
  label: Polar License Keys API
  slug: polar-sh-license-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-license-keys-api-openapi.yml
- filename: polar-sh-meters-api-openapi.yml
  format: yaml
  label: Polar Meters API
  slug: polar-sh-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-meters-api-openapi.yml
- filename: polar-sh-orders-api-openapi.yml
  format: yaml
  label: Polar Orders API
  slug: polar-sh-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-orders-api-openapi.yml
- filename: polar-sh-products-api-openapi.yml
  format: yaml
  label: Polar Products API
  slug: polar-sh-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-products-api-openapi.yml
- filename: polar-sh-subscriptions-api-openapi.yml
  format: yaml
  label: Polar Subscriptions API
  slug: polar-sh-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-subscriptions-api-openapi.yml
- filename: polar-sh-webhooks-api-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: polar-sh-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- Subscription
- Usage-Based Billing
---
