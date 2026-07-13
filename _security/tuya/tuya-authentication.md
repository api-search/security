---
api_key_in:
- header
api_specs:
- filename: tuya-device-management-openapi.yml
  format: yaml
  label: Tuya Device Management API
  slug: device-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuya/refs/heads/main/openapi/tuya-device-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tuya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tuya secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tuya
provider_slug: tuya
scheme_count: 1
schemes:
- description: Tuya API uses HMAC-SHA256 signed requests. Include your Access ID as the client_id header and provide a sign header computed from your Access ID, Access Secret, and timestamp.
  in: header
  name: tuyaApiKey
  parameter: client_id
  sources:
  - openapi/tuya-device-management-openapi.yml
  type: apiKey
slug: tuya-authentication
source_filename: tuya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tuya-device-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tuyaApiKey\n  type: apiKey\n  in: header\n  parameter: client_id\n  description: Tuya API uses HMAC-SHA256 signed requests. Include your Access ID as the client_id\n    header and provide a sign header computed from your Access ID, Access Secret, and timestamp.\n  sources:\n  - openapi/tuya-device-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuya/refs/heads/main/authentication/tuya-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- IoT
- Smart Home
- Devices
- Cloud Platform
- Automation
- Industrial IoT
- Device Management
---
