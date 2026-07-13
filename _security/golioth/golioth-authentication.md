---
api_key_in:
- header
api_specs:
- filename: golioth-openapi.yml
  format: yaml
  label: Golioth Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/openapi/golioth-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Golioth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Golioth secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Golioth
provider_slug: golioth
scheme_count: 2
schemes:
- in: header
  name: API Key
  parameter: x-api-key
  sources:
  - openapi/golioth-openapi.yml
  type: apiKey
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/golioth-openapi.yml
  type: apiKey
slug: golioth-authentication
source_filename: golioth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/golioth-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/golioth-openapi.yml\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/golioth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/authentication/golioth-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- IoT
- Device Management
- Firmware
- Zephyr
- OTA
- Embedded
- Connectivity
---
