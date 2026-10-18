---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dpd-group-countries-api-openapi.yml
  format: yaml
  label: DPD Geo Countries API
  slug: geoapi-countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-countries-api-openapi.yml
- filename: dpd-group-customers-api-openapi.yml
  format: yaml
  label: DPD Geo Customers API
  slug: geoapi-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-customers-api-openapi.yml
- filename: dpd-group-me-api-openapi.yml
  format: yaml
  label: DPD Geo Me API
  slug: geoapi-me
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-me-api-openapi.yml
- filename: dpd-group-parcels-api-openapi.yml
  format: yaml
  label: DPD Geo Parcels API
  slug: geoapi-parcels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-parcels-api-openapi.yml
- filename: dpd-group-pickup-orders-api-openapi.yml
  format: yaml
  label: DPD Geo Pickup Orders API
  slug: geoapi-pickup-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-pickup-orders-api-openapi.yml
- filename: dpd-group-shipments-api-openapi.yml
  format: yaml
  label: DPD Geo Shipments API
  slug: geoapi-shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipments-api-openapi.yml
- filename: dpd-group-shipping-services-api-openapi.yml
  format: yaml
  label: DPD Geo Shipping Services API
  slug: geoapi-shipping-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-services-api-openapi.yml
- filename: dpd-group-shipping-api-openapi.yml
  format: yaml
  label: DPD META-API Shipment
  slug: meta-api-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dpd Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: DPD Group secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DPD Group
provider_slug: dpd-group
scheme_count: 2
schemes:
- description: "Every account will receive its unique API key.  \nThis key is used to uniquely identify your account."
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/dpd-group-countries-api-openapi.yml
  - openapi/dpd-group-customers-api-openapi.yml
  - openapi/dpd-group-me-api-openapi.yml
  - openapi/dpd-group-parcels-api-openapi.yml
  - openapi/dpd-group-pickup-orders-api-openapi.yml
  - openapi/dpd-group-shipments-api-openapi.yml
  - openapi/dpd-group-shipping-services-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dpd-group-shipping-api-openapi.yml
  type: http
slug: dpd-group-authentication
source_filename: dpd-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/dpd-group-countries-api-openapi.yml, openapi/dpd-group-customers-api-openapi.yml,\n  openapi/dpd-group-me-api-openapi.yml, openapi/dpd-group-parcels-api-openapi.yml, openapi/dpd-group-pickup-orders-api-openapi.yml,\n  openapi/dpd-group-shipments-api-openapi.yml, openapi/dpd-group-shipping-api-openapi.yml, openapi/dpd-group-shipping-services-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: \"Every account will receive its unique API key.  \\nThis key is used to uniquely\\\n    \\ identify your account.\"\n  sources:\n  - openapi/dpd-group-countries-api-openapi.yml\n  - openapi/dpd-group-customers-api-openapi.yml\n  - openapi/dpd-group-me-api-openapi.yml\n  - openapi/dpd-group-parcels-api-openapi.yml\n  - openapi/dpd-group-pickup-orders-api-openapi.yml\n  - openapi/dpd-group-shipments-api-openapi.yml\n\
  \  - openapi/dpd-group-shipping-services-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dpd-group-shipping-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/authentication/dpd-group-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Logistics
- Parcel
- Shipping
- Tracking
- Carrier
---
