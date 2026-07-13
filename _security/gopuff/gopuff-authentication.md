---
api_key_in:
- header
api_specs:
- filename: gopuff-fulfillment-openapi.yml
  format: yaml
  label: Powered by Gopuff Fulfillment API
  slug: fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-fulfillment-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gopuff Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gopuff secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gopuff
provider_slug: gopuff
scheme_count: 1
schemes:
- description: Partner API key issued by Gopuff during onboarding to the Powered by Gopuff platform. Keys are scoped to a single partnership/shop.
  in: header
  name: partnerApiKey
  parameter: X-Gopuff-Partner-Key
  sources:
  - openapi/gopuff-fulfillment-openapi.yml
  type: apiKey
slug: gopuff-authentication
source_filename: gopuff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gopuff-fulfillment-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: partnerApiKey\n  type: apiKey\n  in: header\n  parameter: X-Gopuff-Partner-Key\n  description: Partner API key issued by Gopuff during onboarding to the Powered by Gopuff platform.\n    Keys are scoped to a single partnership/shop.\n  sources:\n  - openapi/gopuff-fulfillment-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/authentication/gopuff-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Quick Commerce
- Instant Delivery
- Last Mile
- Grocery
- Fulfillment
- Retail
- Logistics
---
