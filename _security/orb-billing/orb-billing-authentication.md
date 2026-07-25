---
api_key_in: []
api_specs:
- filename: orb-billing-alerts-api-openapi.yml
  format: yaml
  label: Orb Alerts API
  slug: orb-billing-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-alerts-api-openapi.yml
- filename: orb-billing-coupons-api-openapi.yml
  format: yaml
  label: Orb Coupons API
  slug: orb-billing-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-coupons-api-openapi.yml
- filename: orb-billing-credits-api-openapi.yml
  format: yaml
  label: Orb Credits API
  slug: orb-billing-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-credits-api-openapi.yml
- filename: orb-billing-customers-api-openapi.yml
  format: yaml
  label: Orb Customers API
  slug: orb-billing-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-customers-api-openapi.yml
- filename: orb-billing-events-api-openapi.yml
  format: yaml
  label: Orb Events API
  slug: orb-billing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-events-api-openapi.yml
- filename: orb-billing-invoices-api-openapi.yml
  format: yaml
  label: Orb Invoices API
  slug: orb-billing-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-invoices-api-openapi.yml
- filename: orb-billing-items-api-openapi.yml
  format: yaml
  label: Orb Items API
  slug: orb-billing-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-items-api-openapi.yml
- filename: orb-billing-metrics-api-openapi.yml
  format: yaml
  label: Orb Metrics API
  slug: orb-billing-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-metrics-api-openapi.yml
- filename: orb-billing-plans-api-openapi.yml
  format: yaml
  label: Orb Plans API
  slug: orb-billing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-plans-api-openapi.yml
- filename: orb-billing-prices-api-openapi.yml
  format: yaml
  label: Orb Prices API
  slug: orb-billing-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-prices-api-openapi.yml
- filename: orb-billing-subscriptions-api-openapi.yml
  format: yaml
  label: Orb Subscriptions API
  slug: orb-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orb Billing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orb secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orb
provider_slug: orb-billing
scheme_count: 1
schemes:
- description: 'Authenticate with an Orb API key sent as a Bearer token in the Authorization header: `Authorization: Bearer <ORB_API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/orb-billing-openapi.yml
  type: http
slug: orb-billing-authentication
source_filename: orb-billing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orb-billing-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with an Orb API key sent as a Bearer token in the Authorization\n    header: `Authorization: Bearer <ORB_API_KEY>`.'\n  sources:\n  - openapi/orb-billing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/authentication/orb-billing-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Usage-Based Billing
- Metering
- Subscriptions
- Invoicing
- FinOps
---
