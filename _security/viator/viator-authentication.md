---
api_key_in:
- header
- query
api_specs:
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Products API
  slug: viator-partner-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Availability API
  slug: viator-partner-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Bookings API
  slug: viator-partner-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Payments API
  slug: viator-partner-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Attractions API
  slug: viator-partner-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Auxiliary API
  slug: viator-partner-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-reservation-system-api-openapi.json
  format: json
  label: Viator Reservation System API
  slug: viator-reservation-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-reservation-system-api-openapi.json
- filename: viator-merchant-api-v1-openapi.json
  format: json
  label: Viator Merchant API v1
  slug: viator-merchant-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-merchant-api-v1-openapi.json
- filename: viator-affiliate-api-v1-openapi.json
  format: json
  label: Viator Affiliate API v1
  slug: viator-affiliate-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-affiliate-api-v1-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Viator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Viator secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Viator
provider_slug: viator
scheme_count: 3
schemes:
- in: query
  name: Legacy-API-key
  parameter: apiKey
  sources:
  - openapi/viator-affiliate-api-v1-openapi.json
  - openapi/viator-merchant-api-v1-openapi.json
  type: apiKey
- in: header
  name: API-key
  parameter: exp-api-key
  sources:
  - openapi/viator-affiliate-api-v1-openapi.json
  - openapi/viator-merchant-api-v1-openapi.json
  - openapi/viator-partner-api-v2-openapi.json
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/viator-reservation-system-api-openapi.json
  type: apiKey
slug: viator-authentication
source_filename: viator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/viator-affiliate-api-v1-openapi.json, openapi/viator-merchant-api-v1-openapi.json,\n  openapi/viator-partner-api-v2-openapi.json, openapi/viator-reservation-system-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: Legacy-API-key\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/viator-affiliate-api-v1-openapi.json\n  - openapi/viator-merchant-api-v1-openapi.json\n- name: API-key\n  type: apiKey\n  in: header\n  parameter: exp-api-key\n  sources:\n  - openapi/viator-affiliate-api-v1-openapi.json\n  - openapi/viator-merchant-api-v1-openapi.json\n  - openapi/viator-partner-api-v2-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/viator-reservation-system-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/authentication/viator-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Travel
- United States
- Tours and Activities
- Experience
- OTA
- Booking
- Distribution
- Marketplace
- Affiliates
- Hospitality
---
