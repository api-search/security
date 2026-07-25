---
api_key_in: []
api_specs:
- filename: metronome-alerts-api-openapi.yml
  format: yaml
  label: Metronome Alerts API
  slug: metronome-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-alerts-api-openapi.yml
- filename: metronome-billable-metrics-api-openapi.yml
  format: yaml
  label: Metronome Billable Metrics API
  slug: metronome-billable-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-billable-metrics-api-openapi.yml
- filename: metronome-contracts-api-openapi.yml
  format: yaml
  label: Metronome Contracts API
  slug: metronome-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-contracts-api-openapi.yml
- filename: metronome-credits-and-commits-api-openapi.yml
  format: yaml
  label: Metronome Credits and commits API
  slug: metronome-credits-and-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-credits-and-commits-api-openapi.yml
- filename: metronome-custom-fields-api-openapi.yml
  format: yaml
  label: Metronome Custom fields API
  slug: metronome-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-custom-fields-api-openapi.yml
- filename: metronome-customers-api-openapi.yml
  format: yaml
  label: Metronome Customers API
  slug: metronome-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-customers-api-openapi.yml
- filename: metronome-integrations-api-openapi.yml
  format: yaml
  label: Metronome Integrations API
  slug: metronome-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-integrations-api-openapi.yml
- filename: metronome-invoices-api-openapi.yml
  format: yaml
  label: Metronome Invoices API
  slug: metronome-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-invoices-api-openapi.yml
- filename: metronome-named-schedules-api-openapi.yml
  format: yaml
  label: Metronome Named schedules API
  slug: metronome-named-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-named-schedules-api-openapi.yml
- filename: metronome-notifications-api-openapi.yml
  format: yaml
  label: Metronome Notifications API
  slug: metronome-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-notifications-api-openapi.yml
- filename: metronome-packages-api-openapi.yml
  format: yaml
  label: Metronome Packages API
  slug: metronome-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-packages-api-openapi.yml
- filename: metronome-payments-api-openapi.yml
  format: yaml
  label: Metronome Payments API
  slug: metronome-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-payments-api-openapi.yml
- filename: metronome-products-api-openapi.yml
  format: yaml
  label: Metronome Products API
  slug: metronome-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-products-api-openapi.yml
- filename: metronome-rate-cards-api-openapi.yml
  format: yaml
  label: Metronome Rate cards API
  slug: metronome-rate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-rate-cards-api-openapi.yml
- filename: metronome-security-api-openapi.yml
  format: yaml
  label: Metronome Security API
  slug: metronome-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-security-api-openapi.yml
- filename: metronome-settings-api-openapi.yml
  format: yaml
  label: Metronome Settings API
  slug: metronome-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-settings-api-openapi.yml
- filename: metronome-threshold-billing-api-openapi.yml
  format: yaml
  label: Metronome Threshold billing API
  slug: metronome-threshold-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-threshold-billing-api-openapi.yml
- filename: metronome-usage-api-openapi.yml
  format: yaml
  label: Metronome Usage API
  slug: metronome-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Metronome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metronome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metronome
provider_slug: metronome
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/metronome-openapi.json
  type: http
slug: metronome-authentication
source_filename: metronome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metronome-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/metronome-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/authentication/metronome-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- FinOps
- Metering
- Pricing
- Usage-Based Billing
---
