---
api_key_in:
- header
api_specs:
- filename: spoton-availability-api-openapi.yml
  format: yaml
  label: SpotOn Availability API
  slug: spoton-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-availability-api-openapi.yml
- filename: spoton-cash-deposits-api-openapi.yml
  format: yaml
  label: SpotOn Cash Deposits API
  slug: spoton-cash-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-cash-deposits-api-openapi.yml
- filename: spoton-employees-api-openapi.yml
  format: yaml
  label: SpotOn Employees API
  slug: spoton-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-employees-api-openapi.yml
- filename: spoton-job-positions-api-openapi.yml
  format: yaml
  label: SpotOn Job Positions API
  slug: spoton-job-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-job-positions-api-openapi.yml
- filename: spoton-locations-api-openapi.yml
  format: yaml
  label: SpotOn Locations API
  slug: spoton-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-locations-api-openapi.yml
- filename: spoton-menu-items-api-openapi.yml
  format: yaml
  label: SpotOn Menu Items API
  slug: spoton-menu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-menu-items-api-openapi.yml
- filename: spoton-order-types-api-openapi.yml
  format: yaml
  label: SpotOn Order Types API
  slug: spoton-order-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-order-types-api-openapi.yml
- filename: spoton-orders-api-openapi.yml
  format: yaml
  label: SpotOn Orders API
  slug: spoton-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-orders-api-openapi.yml
- filename: spoton-paid-in-outs-api-openapi.yml
  format: yaml
  label: SpotOn Paid In Outs API
  slug: spoton-paid-in-outs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-paid-in-outs-api-openapi.yml
- filename: spoton-payment-options-api-openapi.yml
  format: yaml
  label: SpotOn Payment Options API
  slug: spoton-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-payment-options-api-openapi.yml
- filename: spoton-report-categories-api-openapi.yml
  format: yaml
  label: SpotOn Report Categories API
  slug: spoton-report-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-report-categories-api-openapi.yml
- filename: spoton-reservations-api-openapi.yml
  format: yaml
  label: SpotOn Reservations API
  slug: spoton-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-reservations-api-openapi.yml
- filename: spoton-restaurants-api-openapi.yml
  format: yaml
  label: SpotOn Restaurants API
  slug: spoton-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-restaurants-api-openapi.yml
- filename: spoton-time-clock-entries-api-openapi.yml
  format: yaml
  label: SpotOn Time Clock Entries API
  slug: spoton-time-clock-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-time-clock-entries-api-openapi.yml
- filename: spoton-waitlist-api-openapi.yml
  format: yaml
  label: SpotOn Waitlist API
  slug: spoton-waitlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-waitlist-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spoton Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpotOn secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpotOn
provider_slug: spoton
scheme_count: 1
schemes:
- description: API key scoped to specific restaurants.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/spoton-reserve-openapi-original.yml
  - openapi/spoton-restaurant-pos-export-openapi-original.yml
  type: apiKey
slug: spoton-authentication
source_filename: spoton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spoton-reserve-openapi-original.yml, openapi/spoton-restaurant-pos-export-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key scoped to specific restaurants.\n  sources:\n  - openapi/spoton-reserve-openapi-original.yml\n  - openapi/spoton-restaurant-pos-export-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/authentication/spoton-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Point of Sale
- Payments
- Online Ordering
- Reservations
- Reporting
---
