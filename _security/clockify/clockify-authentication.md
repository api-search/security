---
api_key_in:
- header
api_specs:
- filename: clockify-openapi.json
  format: json
  label: Clockify REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clockify/refs/heads/main/openapi/clockify-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clockify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clockify secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clockify
provider_slug: clockify
scheme_count: 3
schemes:
- in: header
  name: AddonKeyAuth
  parameter: x-addon-token
  sources:
  - openapi/clockify-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/clockify-openapi.json
  type: apiKey
- in: header
  name: MarketplaceKeyAuth
  parameter: x-marketplace-token
  sources:
  - openapi/clockify-openapi.json
  type: apiKey
slug: clockify-authentication
source_filename: clockify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clockify-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AddonKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-addon-token\n  sources:\n  - openapi/clockify-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/clockify-openapi.json\n- name: MarketplaceKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-marketplace-token\n  sources:\n  - openapi/clockify-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockify/refs/heads/main/authentication/clockify-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Time Tracking
- Timesheets
- Productivity
- Project Management
- Reporting
- Invoicing
- Workforce
---
