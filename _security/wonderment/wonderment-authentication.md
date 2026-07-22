---
api_key_in:
- header
api_specs:
- filename: wonderment-openapi.json
  format: json
  label: Wonderment API
  slug: wonderment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/openapi/wonderment-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wonderment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wonderment secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wonderment
provider_slug: wonderment
scheme_count: 1
schemes:
- description: 'Wonderment API access token. Format: sk_live_<shop>_<secret>. Send in the X-Wonderment-Access-Token header over HTTPS.'
  in: header
  name: apiKeyHeader
  parameter: X-Wonderment-Access-Token
  sources:
  - openapi/wonderment-openapi.json
  type: apiKey
slug: wonderment-authentication
source_filename: wonderment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wonderment-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Wonderment-Access-Token\n  description: 'Wonderment API access token. Format: sk_live_<shop>_<secret>. Send in the X-Wonderment-Access-Token\n    header over HTTPS.'\n  sources:\n  - openapi/wonderment-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/authentication/wonderment-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ecommerce
- Order Tracking
- Post-Purchase
- Shipping
- Logistics
- Shopify
- Webhooks
---
