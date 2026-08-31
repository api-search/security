---
api_key_in:
- header
- query
api_specs:
- filename: viator-attraction-services-api-openapi.yml
  format: yaml
  label: Viator Attraction services API
  slug: viator-attraction-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-attraction-services-api-openapi.yml
- filename: viator-attractions-api-openapi.yml
  format: yaml
  label: Viator Attractions API
  slug: viator-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-attractions-api-openapi.yml
- filename: viator-auxiliary-api-openapi.yml
  format: yaml
  label: Viator Auxiliary API
  slug: viator-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-auxiliary-api-openapi.yml
- filename: viator-availability-api-openapi.yml
  format: yaml
  label: Viator Availability API
  slug: viator-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-availability-api-openapi.yml
- filename: viator-booking-services-api-openapi.yml
  format: yaml
  label: Viator Booking services API
  slug: viator-booking-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-booking-services-api-openapi.yml
- filename: viator-bookings-api-openapi.yml
  format: yaml
  label: Viator Bookings API
  slug: viator-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-bookings-api-openapi.yml
- filename: viator-deprecated-api-openapi.yml
  format: yaml
  label: Viator Deprecated API
  slug: viator-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-deprecated-api-openapi.yml
- filename: viator-deprecated-services-api-openapi.yml
  format: yaml
  label: Viator Deprecated services API
  slug: viator-deprecated-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-deprecated-services-api-openapi.yml
- filename: viator-general-services-api-openapi.yml
  format: yaml
  label: Viator General services API
  slug: viator-general-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-general-services-api-openapi.yml
- filename: viator-payments-api-openapi.yml
  format: yaml
  label: Viator Payments API
  slug: viator-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-payments-api-openapi.yml
- filename: viator-product-services-api-openapi.yml
  format: yaml
  label: Viator Product services API
  slug: viator-product-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-product-services-api-openapi.yml
- filename: viator-products-api-openapi.yml
  format: yaml
  label: Viator Products API
  slug: viator-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-products-api-openapi.yml
- filename: viator-reservation-system-apis-api-openapi.yml
  format: yaml
  label: Viator Reservation system APIs API
  slug: viator-reservation-system-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-reservation-system-apis-api-openapi.yml
- filename: viator-support-services-api-openapi.yml
  format: yaml
  label: Viator Support services API
  slug: viator-support-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-support-services-api-openapi.yml
- filename: viator-taxonomy-services-api-openapi.yml
  format: yaml
  label: Viator Taxonomy services API
  slug: viator-taxonomy-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-taxonomy-services-api-openapi.yml
- filename: viator-utility-services-api-openapi.yml
  format: yaml
  label: Viator Utility services API
  slug: viator-utility-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-utility-services-api-openapi.yml
- filename: viator-viator-apis-api-openapi.yml
  format: yaml
  label: Viator Viator APIs API
  slug: viator-viator-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-viator-apis-api-openapi.yml
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
