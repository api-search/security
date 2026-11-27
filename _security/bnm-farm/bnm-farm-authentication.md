---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bnm-farm-free-api-openapi.yml
  format: yaml
  label: BNM Data Shop Free API
  slug: bnm-farm-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bnm-farm/openapi/bnm-farm-free-api-openapi.yml
- filename: bnm-farm-paid-api-openapi.yml
  format: yaml
  label: BNM Data Shop Paid API
  slug: bnm-farm-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bnm-farm/openapi/bnm-farm-paid-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BNM Data Shop Authentication
name_suffix: Authentication
oauth_flows: []
overview: BNM Data Shop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BNM Data Shop
provider_slug: bnm-farm
scheme_count: 1
schemes:
- description: x402 payment payload. Unpaid GET returns HTTP 402 with PAYMENT-REQUIRED.
  in: header
  name: x402
  parameter: X-PAYMENT
  sources:
  - openapi/bnm-farm-openapi.json
  - openapi/openapi.json
  type: apiKey
slug: bnm-farm-authentication
source_filename: bnm-farm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bnm-farm-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 payment payload. Unpaid GET returns HTTP 402 with PAYMENT-REQUIRED.\n  sources:\n  - openapi/bnm-farm-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bnm-farm/authentication/bnm-farm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data
- Marketplace
- Compliance
- Agents
---
