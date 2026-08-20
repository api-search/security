---
api_key_in:
- header
api_specs:
- filename: spreadshirt-articles-api-openapi.yml
  format: yaml
  label: Spreadshirt Articles API
  slug: spreadshirt-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-articles-api-openapi.yml
- filename: spreadshirt-authentication-api-openapi.yml
  format: yaml
  label: Spreadshirt Authentication API
  slug: spreadshirt-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-authentication-api-openapi.yml
- filename: spreadshirt-designs-api-openapi.yml
  format: yaml
  label: Spreadshirt Designs API
  slug: spreadshirt-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-designs-api-openapi.yml
- filename: spreadshirt-orders-api-openapi.yml
  format: yaml
  label: Spreadshirt Orders API
  slug: spreadshirt-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-orders-api-openapi.yml
- filename: spreadshirt-product-types-api-openapi.yml
  format: yaml
  label: Spreadshirt Product Types API
  slug: spreadshirt-product-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-product-types-api-openapi.yml
- filename: spreadshirt-stocks-api-openapi.yml
  format: yaml
  label: Spreadshirt Stocks API
  slug: spreadshirt-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-stocks-api-openapi.yml
- filename: spreadshirt-subscriptions-api-openapi.yml
  format: yaml
  label: Spreadshirt Subscriptions API
  slug: spreadshirt-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-subscriptions-api-openapi.yml
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
- E-Commerce
- Apparel
- Custom Merchandise
- Fulfillment
- Dropshipping
- Webhook
---
