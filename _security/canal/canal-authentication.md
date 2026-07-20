---
api_key_in:
- header
api_specs:
- filename: canal-openapi-original.yml
  format: yaml
  label: Rokt Catalog Platform API
  slug: rokt-catalog-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Canal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canal secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canal
provider_slug: canal
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/canal-openapi-original.yml
  type: http
- in: header
  name: platformAppId
  parameter: X-CANAL-APP-ID
  sources:
  - openapi/canal-openapi-original.yml
  type: apiKey
- in: header
  name: platformAppToken
  parameter: X-CANAL-APP-TOKEN
  sources:
  - openapi/canal-openapi-original.yml
  type: apiKey
slug: canal-authentication
source_filename: canal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/canal-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/canal-openapi-original.yml\n- name: platformAppId\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-ID\n  sources:\n  - openapi/canal-openapi-original.yml\n- name: platformAppToken\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-TOKEN\n  sources:\n  - openapi/canal-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/authentication/canal-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- eCommerce
- Dropshipping
- Marketplace
- Commerce
- Retail
- Fulfillment
- Orders
- Products
- Webhooks
---
