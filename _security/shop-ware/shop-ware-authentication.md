---
api_key_in:
- header
api_specs:
- filename: shop-ware-v2-openapi-original.yml
  format: yaml
  label: Shop-Ware Partner API V2
  slug: shop-ware-partner-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/openapi/shop-ware-v2-openapi-original.yml
- filename: shop-ware-v1-openapi-original.yml
  format: yaml
  label: Shop-Ware Partner API V1
  slug: shop-ware-partner-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/openapi/shop-ware-v1-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shop Ware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shop-Ware secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shop-Ware
provider_slug: shop-ware
scheme_count: 2
schemes:
- in: header
  name: api_partner_id
  parameter: X-Api-Partner-Id
  sources:
  - openapi/shop-ware-v1-openapi-original.yml
  - openapi/shop-ware-v2-openapi-original.yml
  type: apiKey
- in: header
  name: api_secret
  parameter: X-Api-Secret
  sources:
  - openapi/shop-ware-v1-openapi-original.yml
  - openapi/shop-ware-v2-openapi-original.yml
  type: apiKey
slug: shop-ware-authentication
source_filename: shop-ware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shop-ware-v1-openapi-original.yml, openapi/shop-ware-v2-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_partner_id\n  type: apiKey\n  in: header\n  parameter: X-Api-Partner-Id\n  sources:\n  - openapi/shop-ware-v1-openapi-original.yml\n  - openapi/shop-ware-v2-openapi-original.yml\n- name: api_secret\n  type: apiKey\n  in: header\n  parameter: X-Api-Secret\n  sources:\n  - openapi/shop-ware-v1-openapi-original.yml\n  - openapi/shop-ware-v2-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/authentication/shop-ware-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Automotive
- Auto Repair
- Shop Management
- Repair Orders
- Field Service
- SaaS
- Webhooks
- Payments
---
