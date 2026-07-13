---
api_key_in:
- query
api_specs:
- filename: shippingeasy-customer-api-openapi.yml
  format: yaml
  label: ShippingEasy Customer API
  slug: shippingeasy-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/openapi/shippingeasy-customer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shippingeasy Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShippingEasy secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShippingEasy
provider_slug: shippingeasy
scheme_count: 3
schemes:
- description: Account API key. Generated at https://app.shippingeasy.com/settings/api_credentials.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/shippingeasy-customer-api-openapi.yml
  type: apiKey
- description: Unix epoch seconds when the request signature was generated.
  in: query
  name: apiTimestamp
  parameter: api_timestamp
  sources:
  - openapi/shippingeasy-customer-api-openapi.yml
  type: apiKey
- description: HMAC-SHA256 hex digest of the canonical request string computed with the account's API secret.
  in: query
  name: apiSignature
  parameter: api_signature
  sources:
  - openapi/shippingeasy-customer-api-openapi.yml
  type: apiKey
slug: shippingeasy-authentication
source_filename: shippingeasy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shippingeasy-customer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Account API key. Generated at https://app.shippingeasy.com/settings/api_credentials.\n  sources:\n  - openapi/shippingeasy-customer-api-openapi.yml\n- name: apiTimestamp\n  type: apiKey\n  in: query\n  parameter: api_timestamp\n  description: Unix epoch seconds when the request signature was generated.\n  sources:\n  - openapi/shippingeasy-customer-api-openapi.yml\n- name: apiSignature\n  type: apiKey\n  in: query\n  parameter: api_signature\n  description: HMAC-SHA256 hex digest of the canonical request string computed with the account's\n    API secret.\n  sources:\n  - openapi/shippingeasy-customer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/authentication/shippingeasy-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Shipping
- Logistics
- Multi-Carrier
- Labels
- Order Management
- Ecommerce
- Auctane
- Stamps.com
---
