---
api_key_in:
- header
api_specs:
- filename: wetravel-access-token-api-openapi.yml
  format: yaml
  label: WeTravel Access token API
  slug: wetravel-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-access-token-api-openapi.yml
- filename: wetravel-add-ons-api-openapi.yml
  format: yaml
  label: WeTravel Add-ons API
  slug: wetravel-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-add-ons-api-openapi.yml
- filename: wetravel-discounts-api-openapi.yml
  format: yaml
  label: WeTravel Discounts API
  slug: wetravel-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-discounts-api-openapi.yml
- filename: wetravel-images-api-openapi.yml
  format: yaml
  label: WeTravel Images API
  slug: wetravel-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-images-api-openapi.yml
- filename: wetravel-included-items-api-openapi.yml
  format: yaml
  label: WeTravel Included items API
  slug: wetravel-included-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-included-items-api-openapi.yml
- filename: wetravel-leads-api-openapi.yml
  format: yaml
  label: WeTravel Leads API
  slug: wetravel-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-leads-api-openapi.yml
- filename: wetravel-not-included-items-api-openapi.yml
  format: yaml
  label: WeTravel Not Included items API
  slug: wetravel-not-included-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-not-included-items-api-openapi.yml
- filename: wetravel-orders-api-openapi.yml
  format: yaml
  label: WeTravel Orders API
  slug: wetravel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-orders-api-openapi.yml
- filename: wetravel-packages-api-openapi.yml
  format: yaml
  label: WeTravel Packages API
  slug: wetravel-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-packages-api-openapi.yml
- filename: wetravel-paragraphs-api-openapi.yml
  format: yaml
  label: WeTravel Paragraphs API
  slug: wetravel-paragraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-paragraphs-api-openapi.yml
- filename: wetravel-participant-information-api-openapi.yml
  format: yaml
  label: WeTravel Participant Information API
  slug: wetravel-participant-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-participant-information-api-openapi.yml
- filename: wetravel-payment-links-api-openapi.yml
  format: yaml
  label: WeTravel Payment Links API
  slug: wetravel-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-payment-links-api-openapi.yml
- filename: wetravel-payment-plans-api-openapi.yml
  format: yaml
  label: WeTravel Payment Plans API
  slug: wetravel-payment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-payment-plans-api-openapi.yml
- filename: wetravel-suppliers-api-openapi.yml
  format: yaml
  label: WeTravel Suppliers API
  slug: wetravel-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-suppliers-api-openapi.yml
- filename: wetravel-transactions-api-openapi.yml
  format: yaml
  label: WeTravel Transactions API
  slug: wetravel-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-transactions-api-openapi.yml
- filename: wetravel-trip-overview-api-openapi.yml
  format: yaml
  label: WeTravel Trip Overview API
  slug: wetravel-trip-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-trip-overview-api-openapi.yml
- filename: wetravel-trips-api-openapi.yml
  format: yaml
  label: WeTravel Trips API
  slug: wetravel-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-trips-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wetravel Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeTravel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WeTravel
provider_slug: wetravel
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wetravel-partner-openapi.json
  type: http
- in: header
  name: tokenAuth
  parameter: X-Api-Key
  sources:
  - openapi/wetravel-partner-openapi.json
  type: apiKey
slug: wetravel-authentication
source_filename: wetravel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wetravel-partner-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wetravel-partner-openapi.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/wetravel-partner-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/authentication/wetravel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Business Applications
- Travel
- Booking
- Payments
- Trip Management
- Tour Operators
- Travel Technology
---
