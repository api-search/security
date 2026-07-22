---
api_key_in:
- header
api_specs:
- filename: pointcheckout-merchant-api-openapi.yml
  format: yaml
  label: PointCheckout Merchant API
  slug: pointcheckout-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointcheckout/refs/heads/main/openapi/pointcheckout-merchant-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pointcheckout Authentication
name_suffix: Authentication
oauth_flows: []
overview: PointCheckout secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PointCheckout
provider_slug: pointcheckout
scheme_count: 2
schemes:
- in: header
  name: ApiKey
  parameter: X-PointCheckout-Api-Key
  sources:
  - openapi/pointcheckout-merchant-api-openapi.yml
  type: apiKey
- in: header
  name: ApiSecret
  parameter: X-PointCheckout-Api-Secret
  sources:
  - openapi/pointcheckout-merchant-api-openapi.yml
  type: apiKey
slug: pointcheckout-authentication
source_filename: pointcheckout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pointcheckout-merchant-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-PointCheckout-Api-Key\n  sources:\n  - openapi/pointcheckout-merchant-api-openapi.yml\n- name: ApiSecret\n  type: apiKey\n  in: header\n  parameter: X-PointCheckout-Api-Secret\n  sources:\n  - openapi/pointcheckout-merchant-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointcheckout/refs/heads/main/authentication/pointcheckout-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Checkout
- Subscriptions
- Rewards
- Loyalty
- Webhooks
- MENA
- E-Commerce
---
