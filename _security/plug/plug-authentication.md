---
api_key_in:
- header
api_specs:
- filename: plug-openapi-original.yml
  format: yaml
  label: Malga API
  slug: malga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Plug Authentication
name_suffix: Authentication
oauth_flows: []
overview: Malga secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Malga
provider_slug: plug
scheme_count: 2
schemes:
- in: header
  name: X-Client-ID
  parameter: X-Client-Id
  sources:
  - openapi/plug-openapi-original.yml
  type: apiKey
- in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/plug-openapi-original.yml
  type: apiKey
slug: plug-authentication
source_filename: plug-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/plug-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Client-ID\n  type: apiKey\n  in: header\n  parameter: X-Client-Id\n  sources:\n  - openapi/plug-openapi-original.yml\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/plug-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/authentication/plug-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Payment Orchestration
- Payment Gateway
- Fintech
- Pix
- Tokenization
- Subscriptions
- Brazil
---
