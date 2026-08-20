---
api_key_in: []
api_specs:
- filename: octane-admin-api-openapi.yml
  format: yaml
  label: Octane Admin API
  slug: octane-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-admin-api-openapi.yml
- filename: octane-avalara-api-openapi.yml
  format: yaml
  label: Octane Avalara API
  slug: octane-avalara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-avalara-api-openapi.yml
- filename: octane-billing-settings-api-openapi.yml
  format: yaml
  label: Octane Billing Settings API
  slug: octane-billing-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-billing-settings-api-openapi.yml
- filename: octane-coupons-api-openapi.yml
  format: yaml
  label: Octane Coupons API
  slug: octane-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-coupons-api-openapi.yml
- filename: octane-credits-api-openapi.yml
  format: yaml
  label: Octane Credits API
  slug: octane-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-credits-api-openapi.yml
- filename: octane-customer-portal-api-openapi.yml
  format: yaml
  label: Octane Customer Portal API
  slug: octane-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-customer-portal-api-openapi.yml
- filename: octane-customers-api-openapi.yml
  format: yaml
  label: Octane Customers API
  slug: octane-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-customers-api-openapi.yml
- filename: octane-features-api-openapi.yml
  format: yaml
  label: Octane Features API
  slug: octane-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-features-api-openapi.yml
- filename: octane-invoices-api-openapi.yml
  format: yaml
  label: Octane Invoices API
  slug: octane-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-invoices-api-openapi.yml
- filename: octane-live-measurements-api-openapi.yml
  format: yaml
  label: Octane Live Measurements API
  slug: octane-live-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-live-measurements-api-openapi.yml
- filename: octane-measurements-api-openapi.yml
  format: yaml
  label: Octane Measurements API
  slug: octane-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-measurements-api-openapi.yml
- filename: octane-meters-api-openapi.yml
  format: yaml
  label: Octane Meters API
  slug: octane-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-meters-api-openapi.yml
- filename: octane-price-plans-api-openapi.yml
  format: yaml
  label: Octane Price Plans API
  slug: octane-price-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-price-plans-api-openapi.yml
- filename: octane-refunds-api-openapi.yml
  format: yaml
  label: Octane Refunds API
  slug: octane-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-refunds-api-openapi.yml
- filename: octane-revenue-recognition-api-openapi.yml
  format: yaml
  label: Octane Revenue Recognition API
  slug: octane-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-revenue-recognition-api-openapi.yml
- filename: octane-subscriptions-api-openapi.yml
  format: yaml
  label: Octane Subscriptions API
  slug: octane-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-subscriptions-api-openapi.yml
- filename: octane-webhooks-api-openapi.yml
  format: yaml
  label: Octane Webhooks API
  slug: octane-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Octane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octane secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octane
provider_slug: octane
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: BearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/octane-octane-rest-api-openapi.yml
  type: http
slug: octane-authentication
source_filename: octane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octane-octane-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/octane-octane-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/authentication/octane-authentication.yml
summary_line: http · 1 scheme
tags:
- Usage-Based Billing
- Metered Billing
- Pricing Plans
- SaaS Monetization
- Fintech
- Payments
- Usage Tracking
- Meters
- Entitlements
---
