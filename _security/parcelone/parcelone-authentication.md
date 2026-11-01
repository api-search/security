---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: parcelone-closing-api-openapi.yml
  format: yaml
  label: ParcelOne Closing API
  slug: parcelone-closing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-closing-api-openapi.yml
- filename: parcelone-customer-api-openapi.yml
  format: yaml
  label: ParcelOne Customer API
  slug: parcelone-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customer-api-openapi.yml
- filename: parcelone-customs-api-openapi.yml
  format: yaml
  label: ParcelOne Customs API
  slug: parcelone-customs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customs-api-openapi.yml
- filename: parcelone-datetime-api-openapi.yml
  format: yaml
  label: ParcelOne Datetime API
  slug: parcelone-datetime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-datetime-api-openapi.yml
- filename: parcelone-mandator-api-openapi.yml
  format: yaml
  label: ParcelOne Mandator API
  slug: parcelone-mandator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mandator-api-openapi.yml
- filename: parcelone-mobilereturn-api-openapi.yml
  format: yaml
  label: ParcelOne Mobilereturn API
  slug: parcelone-mobilereturn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mobilereturn-api-openapi.yml
- filename: parcelone-profile-api-openapi.yml
  format: yaml
  label: ParcelOne Profile API
  slug: parcelone-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-profile-api-openapi.yml
- filename: parcelone-shipment-api-openapi.yml
  format: yaml
  label: ParcelOne Shipment API
  slug: parcelone-shipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-shipment-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Parcelone Authentication
name_suffix: Authentication
oauth_flows: []
overview: ParcelOne secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ParcelOne
provider_slug: parcelone
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: Apikey
  sources:
  - openapi/parcelone-shipping-openapi.json
  - openapi/parcelone-tracklmc-openapi.json
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/parcelone-shipping-openapi.json
  - openapi/parcelone-tracklmc-openapi.json
  type: http
- bearerFormat: JWT
  name: Bearer_JWT
  scheme: bearer
  sources:
  - openapi/parcelone-shipping-openapi.json
  - openapi/parcelone-tracklmc-openapi.json
  type: http
slug: parcelone-authentication
source_filename: parcelone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/parcelone-shipping-openapi.json, openapi/parcelone-tracklmc-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Apikey\n  sources:\n  - openapi/parcelone-shipping-openapi.json\n  - openapi/parcelone-tracklmc-openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/parcelone-shipping-openapi.json\n  - openapi/parcelone-tracklmc-openapi.json\n- name: Bearer_JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/parcelone-shipping-openapi.json\n  - openapi/parcelone-tracklmc-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/parcelone/authentication/parcelone-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Logistics
- Shipping
- E-commerce
- Fulfillment
- International
---
