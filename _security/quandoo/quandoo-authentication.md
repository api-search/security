---
api_key_in:
- header
api_specs:
- filename: quandoo-availabilities-api-openapi.yml
  format: yaml
  label: Quandoo Availabilities API
  slug: quandoo-availabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-availabilities-api-openapi.yml
- filename: quandoo-customers-api-openapi.yml
  format: yaml
  label: Quandoo Customers API
  slug: quandoo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-customers-api-openapi.yml
- filename: quandoo-merchants-api-openapi.yml
  format: yaml
  label: Quandoo Merchants API
  slug: quandoo-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-merchants-api-openapi.yml
- filename: quandoo-reservation-enquiries-api-openapi.yml
  format: yaml
  label: Quandoo Reservation Enquiries API
  slug: quandoo-reservation-enquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservation-enquiries-api-openapi.yml
- filename: quandoo-reservation-settings-api-openapi.yml
  format: yaml
  label: Quandoo Reservation Settings API
  slug: quandoo-reservation-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservation-settings-api-openapi.yml
- filename: quandoo-reservations-api-openapi.yml
  format: yaml
  label: Quandoo Reservations API
  slug: quandoo-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservations-api-openapi.yml
- filename: quandoo-reservations-tags-api-openapi.yml
  format: yaml
  label: Quandoo Reservations Tags API
  slug: quandoo-reservations-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservations-tags-api-openapi.yml
- filename: quandoo-reviews-api-openapi.yml
  format: yaml
  label: Quandoo Reviews API
  slug: quandoo-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reviews-api-openapi.yml
- filename: quandoo-status-api-openapi.yml
  format: yaml
  label: Quandoo Status API
  slug: quandoo-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-status-api-openapi.yml
- filename: quandoo-validations-api-openapi.yml
  format: yaml
  label: Quandoo Validations API
  slug: quandoo-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-validations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quandoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quandoo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quandoo
provider_slug: quandoo
scheme_count: 1
schemes:
- in: header
  name: API_TOKEN
  parameter: X-Quandoo-AuthToken
  sources:
  - openapi/quandoo-public-partner-api-openapi.yml
  type: apiKey
slug: quandoo-authentication
source_filename: quandoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quandoo-public-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_TOKEN\n  type: apiKey\n  in: header\n  parameter: X-Quandoo-AuthToken\n  sources:\n  - openapi/quandoo-public-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/authentication/quandoo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Reservations
- Booking
- Availability
- Merchants
- Marketplace
---
