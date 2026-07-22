---
api_key_in:
- header
api_specs:
- filename: spreadshirt-spreadconnect-openapi.json
  format: json
  label: SpreadConnect (SPOD) Fulfillment API
  slug: spreadconnect-spod-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-spreadconnect-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spreadshirt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spreadshirt secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spreadshirt
provider_slug: spreadshirt
scheme_count: 1
schemes:
- description: It's necessary to have an authentication token from Spreadconnect. You can generate this token in your Spreadconnect web application. You have to send this token as a header parameter in each request.
  in: header
  name: access_token
  parameter: X-SPOD-ACCESS-TOKEN
  sources:
  - openapi/spreadshirt-spreadconnect-openapi.json
  type: apiKey
slug: spreadshirt-authentication
source_filename: spreadshirt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/spreadshirt-spreadconnect-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: access_token\n  type: apiKey\n  in: header\n  parameter: X-SPOD-ACCESS-TOKEN\n  description: It's necessary to have an authentication token from Spreadconnect. You can generate\n    this token in your Spreadconnect web application. You have to send this token as a header\n    parameter in each request.\n  sources:\n  - openapi/spreadshirt-spreadconnect-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/authentication/spreadshirt-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Print on Demand
- E-commerce
- Apparel
- Custom Merchandise
- Fulfillment
- Dropshipping
- Webhooks
---
