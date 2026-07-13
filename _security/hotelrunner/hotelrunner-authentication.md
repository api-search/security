---
api_key_in:
- query
api_specs:
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Inventory API
  slug: hotelrunner-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reservations API
  slug: hotelrunner-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Channels API
  slug: hotelrunner-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reference Data API
  slug: hotelrunner-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hotelrunner Authentication
name_suffix: Authentication
oauth_flows: []
overview: HotelRunner secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HotelRunner
provider_slug: hotelrunner
scheme_count: 1
schemes:
- description: API token issued in the property's HotelRunner Partners extranet ("My Property" section) or PMS sandbox account. Always sent together with the hr_id query parameter identifying the property.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/hotelrunner-openapi.yml
  type: apiKey
slug: hotelrunner-authentication
source_filename: hotelrunner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hotelrunner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token issued in the property's HotelRunner Partners extranet (\"My Property\"\n    section) or PMS sandbox account. Always sent together with the hr_id query parameter identifying\n    the property.\n  sources:\n  - openapi/hotelrunner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/authentication/hotelrunner-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Hotel
- Channel Manager
- Booking Engine
- PMS
- Travel
---
