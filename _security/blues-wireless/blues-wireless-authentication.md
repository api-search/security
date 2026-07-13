---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Notehub API
  slug: blues-wireless-notehub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/blues/notehub-js/main/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blues Wireless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blues secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blues
provider_slug: blues-wireless
scheme_count: 1
schemes:
- description: Use a personal access token from notehub.io/api-access
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/blues-wireless-notehub-api-openapi.yml
  type: http
slug: blues-wireless-authentication
source_filename: blues-wireless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blues-wireless-notehub-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: Use a personal access token from notehub.io/api-access\n  sources:\n  - openapi/blues-wireless-notehub-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/authentication/blues-wireless-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Cellular
- Connectivity
- Device Management
- Fleet Management
- Satellite
- LoRa
- WiFi
- Notecard
- Notehub
---
