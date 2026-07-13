---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Choozle Reporting API
  slug: choozle-reporting-api
  spec_type: OpenAPI
  url: https://app.choozle.com/apidoc/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Choozle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Choozle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Choozle
provider_slug: choozle
scheme_count: 1
schemes:
- description: API token obtained from the /authorization endpoint. Valid for 2 hours. Pass the token value as the `token` request header.
  in: header
  name: tokenHeader
  parameter: token
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: choozle-authentication
source_filename: choozle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: token\n  description: API token obtained from the /authorization endpoint. Valid for 2 hours. Pass\n    the token value as the `token` request header.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/authentication/choozle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Advertising
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Audience Targeting
- Display Advertising
- Connected TV
- CTV
- Video Advertising
- Native Advertising
- DOOH
- Reporting
- Real-Time Bidding
- RTB
---
