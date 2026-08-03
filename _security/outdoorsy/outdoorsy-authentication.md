---
api_key_in:
- header
api_specs:
- filename: outdoorsy-openapi-original.json
  format: json
  label: Outdoorsy API
  slug: outdoorsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/openapi/outdoorsy-openapi-original.json
- filename: outdoorsy-search-openapi-original.json
  format: json
  label: Outdoorsy Search API
  slug: outdoorsy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/openapi/outdoorsy-search-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Outdoorsy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outdoorsy secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Outdoorsy
provider_slug: outdoorsy
scheme_count: 2
schemes:
- in: header
  name: API-Key
  parameter: API-Key
  sources:
  - openapi/outdoorsy-openapi-original.json
  type: apiKey
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/outdoorsy-openapi-original.json
  - openapi/outdoorsy-search-openapi-original.json
  type: apiKey
slug: outdoorsy-authentication
source_filename: outdoorsy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/outdoorsy-openapi-original.json, openapi/outdoorsy-search-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API-Key\n  type: apiKey\n  in: header\n  parameter: API-Key\n  sources:\n  - openapi/outdoorsy-openapi-original.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/outdoorsy-openapi-original.json\n  - openapi/outdoorsy-search-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/authentication/outdoorsy-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Travel
- Marketplace
- Rentals
- Recreational Vehicles
- Bookings
- Search
- Payments
- Insurance
- Camping
- Tourism
---
