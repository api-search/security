---
api_key_in:
- header
api_specs:
- filename: axlehire-assignment-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Assignment Information API
  slug: axlehire-assignment-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-assignment-information-api-openapi.yml
- filename: axlehire-driver-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Driver Information API
  slug: axlehire-driver-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-driver-information-api-openapi.yml
- filename: axlehire-partner-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Partner Information API
  slug: axlehire-partner-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-partner-information-api-openapi.yml
- filename: axlehire-shipping-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Shipping Information API
  slug: axlehire-shipping-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-shipping-information-api-openapi.yml
- filename: axlehire-tracking-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Tracking Information API
  slug: axlehire-tracking-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-tracking-information-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Axlehire Authentication
name_suffix: Authentication
oauth_flows: []
overview: AxleHire (Jitsu) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AxleHire (Jitsu)
provider_slug: axlehire
scheme_count: 1
schemes:
- description: '**Authorization header for all calls in format: ''Authorization : Token {YOUR_TOKEN}''**'
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/axlehire-jitsu-rest-api.yml
  type: apiKey
slug: axlehire-authentication
source_filename: axlehire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/axlehire-jitsu-rest-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '**Authorization header for all calls in format: ''Authorization : Token {YOUR_TOKEN}''**'\n  sources:\n  - openapi/axlehire-jitsu-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/authentication/axlehire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Last Mile Delivery
- Shipping
- Parcel
- Transportation
- Supply Chain
- Ecommerce
- Tracking
- Webhooks
---
