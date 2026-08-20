---
api_key_in:
- header
api_specs:
- filename: trend-api-openapi.yml
  format: yaml
  label: Trend API
  slug: trend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trend secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trend
provider_slug: trend
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: access-token
  scheme: bearer
  sources:
  - openapi/trend-api-openapi.yml
  type: http
- in: header
  name: admin-api-key
  parameter: trend-api-key
  sources:
  - openapi/trend-api-openapi.yml
  type: apiKey
slug: trend-authentication
source_filename: trend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/trend-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: access-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/trend-api-openapi.yml\n- name: admin-api-key\n  type: apiKey\n  in: header\n  parameter: trend-api-key\n  sources:\n  - openapi/trend-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/authentication/trend-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- User Generated Content
- Creator Economy
- Content Marketing
- Video Production
- Photography
- Marketing
- E-Commerce
- Creator Marketplace
- Influencer Marketing
- AI Image Generation
- Payments
---
