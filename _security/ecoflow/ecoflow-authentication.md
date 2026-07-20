---
api_key_in:
- header
api_specs:
- filename: ecoflow-iot-openapi.yml
  format: yaml
  label: EcoFlow IoT Open Platform
  slug: ecoflow-iot-open-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecoflow/refs/heads/main/openapi/ecoflow-iot-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ecoflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: EcoFlow secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EcoFlow
provider_slug: ecoflow
scheme_count: 4
schemes:
- description: Access key issued in the EcoFlow developer console.
  in: header
  name: accessKey
  parameter: accessKey
  sources:
  - openapi/ecoflow-iot-openapi.yml
  type: apiKey
- description: Random nonce (typically a 6-digit number) regenerated per request.
  in: header
  name: nonce
  parameter: nonce
  sources:
  - openapi/ecoflow-iot-openapi.yml
  type: apiKey
- description: Unix timestamp in milliseconds at request time.
  in: header
  name: timestamp
  parameter: timestamp
  sources:
  - openapi/ecoflow-iot-openapi.yml
  type: apiKey
- description: HMAC-SHA256 signature (hex) over the ASCII-sorted request parameters concatenated with `accessKey`, `nonce` and `timestamp`, keyed by the secretKey.
  in: header
  name: sign
  parameter: sign
  sources:
  - openapi/ecoflow-iot-openapi.yml
  type: apiKey
slug: ecoflow-authentication
source_filename: ecoflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/ecoflow-iot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  parameter: accessKey\n  description: Access key issued in the EcoFlow developer console.\n  sources:\n  - openapi/ecoflow-iot-openapi.yml\n- name: nonce\n  type: apiKey\n  in: header\n  parameter: nonce\n  description: Random nonce (typically a 6-digit number) regenerated per request.\n  sources:\n  - openapi/ecoflow-iot-openapi.yml\n- name: timestamp\n  type: apiKey\n  in: header\n  parameter: timestamp\n  description: Unix timestamp in milliseconds at request time.\n  sources:\n  - openapi/ecoflow-iot-openapi.yml\n- name: sign\n  type: apiKey\n  in: header\n  parameter: sign\n  description: HMAC-SHA256 signature (hex) over the ASCII-sorted request parameters concatenated\n    with `accessKey`, `nonce` and `timestamp`, keyed by the secretKey.\n  sources:\n  - openapi/ecoflow-iot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecoflow/refs/heads/main/authentication/ecoflow-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Technology
- Energy
- Energy Storage
- Portable Power
- IoT
- Smart Home
- Solar
- Developer API
---
