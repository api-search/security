---
api_key_in:
- header
api_specs:
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Reservations & Bookings API
  slug: ezee-reservations-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Room Inventory & Rates API
  slug: ezee-room-inventory-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Guests & Configuration API
  slug: ezee-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Centrix Channel Manager API
  slug: ezee-channel-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ezee Authentication
name_suffix: Authentication
oauth_flows: []
overview: eZee Technosys secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: eZee Technosys
provider_slug: ezee
scheme_count: 1
schemes:
- description: Property-scoped credentials (HotelCode + AuthCode) provisioned through the YCS Connectivity Portal, supplied per the portal's authentication conventions (commonly carried in the request body and/or as HTTP Basic with a vendor-identifying User-Agent header). Not a self-serve public API key.
  in: header
  name: HotelCodeAuthCode
  parameter: Authorization
  sources:
  - openapi/ezee-openapi.yml
  type: apiKey
slug: ezee-authentication
source_filename: ezee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ezee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HotelCodeAuthCode\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Property-scoped credentials (HotelCode + AuthCode) provisioned through the YCS\n    Connectivity Portal, supplied per the portal's authentication conventions (commonly carried\n    in the request body and/or as HTTP Basic with a vendor-identifying User-Agent header). Not\n    a self-serve public API key.\n  sources:\n  - openapi/ezee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/authentication/ezee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Hotel
- PMS
- Channel Manager
- Reservations
---
