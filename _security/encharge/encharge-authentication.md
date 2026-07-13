---
api_key_in:
- header
api_specs:
- filename: encharge-openapi.yml
  format: yaml
  label: Encharge REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Encharge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Encharge secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Encharge
provider_slug: encharge
scheme_count: 2
schemes:
- in: header
  name: tokenHeader
  parameter: X-Encharge-Token
  sources:
  - openapi/encharge-openapi.yml
  type: apiKey
- name: bearer
  scheme: bearer
  sources:
  - openapi/encharge-openapi.yml
  type: http
slug: encharge-authentication
source_filename: encharge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/encharge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Encharge-Token\n  sources:\n  - openapi/encharge-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/encharge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/authentication/encharge-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- SaaS
- Behavioral Email
- Customer Engagement
---
