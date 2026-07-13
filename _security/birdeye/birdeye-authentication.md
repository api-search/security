---
api_key_in:
- header
api_specs:
- filename: birdeye-birdeye-api-openapi.yml
  format: yaml
  label: Birdeye API
  slug: birdeye-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/birdeye/refs/heads/main/openapi/birdeye-birdeye-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Birdeye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Birdeye secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Birdeye
provider_slug: birdeye
scheme_count: 1
schemes:
- description: Partner specific API key provided by Birdeye for data exchange.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/birdeye-birdeye-api-openapi.yml
  type: apiKey
slug: birdeye-authentication
source_filename: birdeye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/birdeye-birdeye-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Partner specific API key provided by Birdeye for data exchange.\n  sources:\n  - openapi/birdeye-birdeye-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/birdeye/refs/heads/main/authentication/birdeye-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Reputation Management
- Reviews
- Customer Experience
- Surveys
- Messaging
- Multi-Location
- AI
---
