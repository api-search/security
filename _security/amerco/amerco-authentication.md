---
api_key_in:
- header
api_specs:
- filename: amerco-webselfstorage-affiliate-api-v4-openapi.yml
  format: yaml
  label: WebSelfStorage Affiliate API
  slug: webselfstorage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amerco/refs/heads/main/openapi/amerco-webselfstorage-affiliate-api-v4-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amerco Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMERCO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AMERCO
provider_slug: amerco
scheme_count: 1
schemes:
- description: Add "Bearer" followed by space and then your access token to test
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/amerco-webselfstorage-affiliate-api-v3-openapi.yml
  - openapi/amerco-webselfstorage-affiliate-api-v4-openapi.yml
  type: apiKey
slug: amerco-authentication
source_filename: amerco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/amerco-webselfstorage-affiliate-api-v3-openapi.yml, openapi/amerco-webselfstorage-affiliate-api-v4-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Add \"Bearer\" followed by space and then your access token to test\n  sources:\n  - openapi/amerco-webselfstorage-affiliate-api-v3-openapi.yml\n  - openapi/amerco-webselfstorage-affiliate-api-v4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerco/refs/heads/main/authentication/amerco-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Moving
- Storage
- Truck Rental
- Logistics
- Consumer Services
- Fortune 1000
---
