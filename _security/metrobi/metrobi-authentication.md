---
api_key_in:
- header
api_specs:
- filename: metrobi-deliveries-api-openapi.yml
  format: yaml
  label: Metrobi Deliveries API
  slug: metrobi-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/openapi/metrobi-deliveries-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metrobi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metrobi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metrobi
provider_slug: metrobi
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/metrobi-delivery-api-openapi.json
  type: apiKey
slug: metrobi-authentication
source_filename: metrobi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/metrobi-delivery-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/metrobi-delivery-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/authentication/metrobi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Delivery
- Logistics
- Courier
- Last Mile Delivery
- Route Optimization
- Fulfillment
- Local Delivery
- Webhooks
---
